---
api_specs:
- filename: amber-electric-public-api-openapi.json
  format: json
  label: Amber Electric Public API
  slug: amber-electric-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amber-electric/refs/heads/main/openapi/amber-electric-public-api-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issue "amazontrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amber.com.au
  spf: true
hosts:
- cert_expires: Oct 16 06:03:17 2026 GMT
  host: amber.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: app.amber.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: api.amber.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 15:43:02 2026 GMT
  cert_verify: ok
  host: public.cdr.amber.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: Added by hand — the automated probe covers only the first three apis.yml hosts.
  probed: '2026-07-27'
  role: Consumer Data Right public base URI
  tls_version: TLSv1.3
- cert_expires: Jul  2 23:59:59 2027 GMT
  cert_verify: failed anonymously — 20 (unable to get local issuer certificate)
  host: secure.cdr.amber.com.au
  hsts: false
  https: true
  note: 'An anonymous client cannot complete a normal TLS handshake against this host; it is reached with a CDR-issued client certificate under mutual TLS, which is consistent with tls_client_certificate_bound_access_tokens: true in the OpenID Connect discovery document. Recorded as observed, not as a defect.'
  probed: '2026-07-27'
  role: Consumer Data Right token/registration host (accredited recipients only)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amber Electric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amber Electric, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amber Electric
provider_slug: amber-electric
slug: amber-electric-domain-security
source_filename: amber-electric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amber.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 06:03:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.amber.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: false\n- host: api.amber.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: null\n- host: public.cdr.amber.com.au\n  role: Consumer Data Right public base URI\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:43:02 2026 GMT\n  cert_verify: ok\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  probed: '2026-07-27'\n  note: Added by hand — the automated probe covers only the first three apis.yml hosts.\n- host: secure.cdr.amber.com.au\n  role: Consumer Data Right token/registration host (accredited recipients\
  \ only)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul  2 23:59:59 2027 GMT\n  cert_verify: 'failed anonymously — 20 (unable to get local issuer certificate)'\n  hsts: false\n  probed: '2026-07-27'\n  note: >-\n    An anonymous client cannot complete a normal TLS handshake against this\n    host; it is reached with a CDR-issued client certificate under mutual TLS,\n    which is consistent with tls_client_certificate_bound_access_tokens: true in\n    the OpenID Connect discovery document. Recorded as observed, not as a defect.\ndomains:\n- domain: amber.com.au\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amber-electric/refs/heads/main/security/amber-electric-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Australia
- Electricity
- Utilities
- Consumer Data Right
- Energy Markets
- Renewables
- Solar
- Batteries
- DER
- Smart Metering
- Wholesale Pricing
---
