---
api_key_in: []
auth_types:
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Jemena Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jemena secures its APIs with mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Jemena
provider_slug: jemena
scheme_count: 2
schemes:
- description: All client communication to the JEN Utility Server requires a certified PKI certificate to authenticate and identify the client. Certificates are unique per client AND per environment — a staging certificate does not work in production. The handbook documents a native IEEE 2030.5 root CA device certificate profile (Section C1.1) and an intermediate Manufacturer Certificate Authority (MCA) certificate profile (Section C1.2).
  evidence: 'Anonymous GET https://sep2.aws.jemena.com.au:8443/sep2/dcap on 2026-07-27 completes the TLS handshake against a private-PKI certificate (curl ssl_verify_result=19, self-signed certificate in chain — expected for the SEP2 SERCA/MICA hierarchy) and returns HTTP 500 from nginx with verification disabled, because no client certificate was presented. Handbook FAQ 8.7.1 confirms the failure mode: "the remote end closed connection without response" means the request did not include a valid PKI certificate.'
  name: IEEE 2030.5 client certificate (mTLS)
  pki:
    intermediate: MCA / MICA (Manufacturer Certificate Authority) — direct-connected device model
    issuer: Jemena Electricity Networks (JEN) signs the client CSR
    root: SERCA (Smart Energy Root Certificate Authority)
  source: handbook Section 10 Certificate Public Key Infrastructure (PKI)
  type: mutualTLS
- description: A network-layer control applied in addition to mTLS. Clients submit the IP addresses to be whitelisted alongside their Certificate Signing Request. The handbook states IP access restriction is implemented in the non-production/staging environment for onboarding testing, and asks for 7 business days advance notice of any IP change.
  name: Source IP allow-listing
  source: handbook Section 7.1.1 step 2
  type: network
slug: jemena-authentication
source_filename: jemena-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://www.jemena.com.au/siteassets/asset-folder/documents/electricity/embedded-generation/jen-oem-technical-guide_handbook_v1.0.1-final.pdf\ndocs: https://www.jemena.com.au/electricity/solar-connections/victoria-emergency-backstop-mechanism/emergency-backstop-mechanism-documents/\napi: jemena:jemena-csip-aus-utility-server\nnote: >-\n  Jemena publishes no OpenAPI, so this profile is harvested from the prose contract in the public\n  JEN OEM Technical Guide Handbook (v1.0, 12 June 2025) rather than derived from securitySchemes.\n  There is no bearer token, no API key and no OAuth surface anywhere on the JEN Utility Server:\n  identity is a Jemena-signed X.509 client certificate presented in a mutually-authenticated TLS\n  handshake, and the on-the-wire device identity is the LFDI hashed from that certificate.\nsummary:\n  types:\n  - mutualTLS\n  api_key_in: []\n  oauth2_flows: []\n  self_serve: false\n  gate: application-approval\n\
  schemes:\n- name: IEEE 2030.5 client certificate (mTLS)\n  type: mutualTLS\n  description: >-\n    All client communication to the JEN Utility Server requires a certified PKI certificate to\n    authenticate and identify the client. Certificates are unique per client AND per environment —\n    a staging certificate does not work in production. The handbook documents a native IEEE 2030.5\n    root CA device certificate profile (Section C1.1) and an intermediate Manufacturer Certificate\n    Authority (MCA) certificate profile (Section C1.2).\n  source: handbook Section 10 Certificate Public Key Infrastructure (PKI)\n  pki:\n    root: SERCA (Smart Energy Root Certificate Authority)\n    intermediate: MCA / MICA (Manufacturer Certificate Authority) — direct-connected device model\n    issuer: Jemena Electricity Networks (JEN) signs the client CSR\n  evidence: >-\n    Anonymous GET https://sep2.aws.jemena.com.au:8443/sep2/dcap on 2026-07-27 completes the TLS\n    handshake against a private-PKI\
  \ certificate (curl ssl_verify_result=19, self-signed certificate\n    in chain — expected for the SEP2 SERCA/MICA hierarchy) and returns HTTP 500 from nginx with\n    verification disabled, because no client certificate was presented. Handbook FAQ 8.7.1 confirms\n    the failure mode: \"the remote end closed connection without response\" means the request did not\n    include a valid PKI certificate.\n- name: Source IP allow-listing\n  type: network\n  description: >-\n    A network-layer control applied in addition to mTLS. Clients submit the IP addresses to be\n    whitelisted alongside their Certificate Signing Request. The handbook states IP access\n    restriction is implemented in the non-production/staging environment for onboarding testing,\n    and asks for 7 business days advance notice of any IP change.\n  source: handbook Section 7.1.1 step 2\nidentity:\n  device_identifier: LFDI (Long Form Device Identifier)\n  lfdi_definition: >-\n    40 hexadecimal characters, alphanumeric\
  \ only, no special characters, derived by hashing the\n    device X.509 certificate. Handbook FAQ 8.3.1 publishes the generation command verbatim:\n    openssl x509 -outform der -in client-cert.pem | sha256sum | head -c 40 | tr '[a-f]' '[A-F]'\n  direct_device_model: >-\n    Device LFDI is the certificate fingerprint left-truncated to 160 bits (20 octets), expressed as\n    40 hexadecimal digits in groups of four.\n  aggregator_model: >-\n    One certificate represents many downstream sites. Virtual LFDIs are minted by the aggregator:\n    first 32 hex digits are a unique identifier, last 8 hex digits are the provider's IANA Private\n    Enterprise Number (PEN) with leading zeros. Each LFDI and its associated SFDI must be unique.\n  secondary_identifier: SFDI (Short Form Device Identifier), String(12), numeric only\n  site_identifier: >-\n    ConnectionPointID — the 10-digit NMI (National Metering Identifier) plus 1 checksum digit,\n    validated against the JEN NMI database. An invalid\
  \ ConnectionPointID returns HTTP 403.\nregistration:\n  in_band:\n    supported: true\n    scope: aggregator model only\n    note: >-\n      Jemena states in-band registration is supported only for aggregator-model clients and is still\n      under test; additional onboarding tests are required before production use. A 204 No Content on\n      GET /sep2/edev/{x}/rg means the Registration PIN is null/blank/empty and the client should\n      proceed without PIN-based validation.\n  out_of_band:\n    supported: true\n    note: Default path; recommended where the client cannot support the in-band behaviour above.\n  registration_pin:\n    required: false\n    note: >-\n      Optional. Jemena publishes both environment PINs in the public handbook (Section 7.1.1 step 3\n      and FAQ 8.4). The staging value is recorded in sandbox/jemena-sandbox.yml; the production value\n      is left in the source document rather than mirrored here.\nonboarding:\n  self_serve: false\n  contact: emergency.backstop@jemena.com.au\n\
  \  steps:\n  - Be an inverter OEM, gateway manufacturer or aggregator whose product is on the Clean Energy Council list of AS/NZS 4777.2:2020 CSIP-AUS compliant inverters.\n  - Generate a private key.\n  - Submit a Certificate Signing Request plus the IP addresses to whitelist (aggregator model), or an MCA intermediate-CA CSR plus a CA Naming Form (direct-connected device model), by email or file share to emergency.backstop@jemena.com.au.\n  - Receive the JEN-signed certificate, the aggregator LFDI and the registration PIN.\n  - Pass the connectivity test, device registration, discovery test and out-of-band functional tests in the staging environment.\n  - Repeat certificate issuance and testing in the production environment.\n  - Jemena adds the client to its public CSIP-AUS Approved Listing; from 1 July 2025 inverters not on that listing cannot connect or commission.\n  key_custody_warning: >-\n    \"Client must keep their Private Key and JEN issued Certificate in a safe place. If it\
  \ is lost,\n    client must notify JEN to reapply for the certificate. Additional cost will incurred here, up to\n    $3000 USD. The client is responsible for this fee.\" (handbook Sections 7.1.1 and 7.1.2)\nnot_present:\n  oauth2: No OAuth 2.0 authorization server is published or referenced.\n  openid_connect: >-\n    GET https://www.jemena.com.au/.well-known/openid-configuration returned 404 and\n    https://myportal.jemena.com.au/.well-known/openid-configuration returned 403 on 2026-07-27.\n  api_key: No API key scheme is documented anywhere on the JEN Utility Server.\n  scopes: >-\n    No OAuth scope surface exists, so scopes/ is intentionally absent. Authorisation is expressed as\n    certificate validity plus LFDI-to-resource binding — handbook FAQ 8.7.5 documents HTTP 403 as an\n    LFDI mismatch and FAQ 8.7.3 documents HTTP 404 as \"existence confirmation is withheld\" for an\n    unauthorised certificate.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jemena/refs/heads/main/authentication/jemena-authentication.yml
summary_line: mutualTLS · 2 schemes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Grid
- Network Distributor
- DER
- Solar
- Smart Metering
- Demand Response
- IEEE 2030.5
---
