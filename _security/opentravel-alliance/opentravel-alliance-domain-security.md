---
api_specs:
- filename: opentravel-2020a-hotel-descriptive-content-resource-defs-openapi.json
  format: json
  label: OpenTravel 2020A Hotel Descriptive Content Resource
  slug: opentravel-2020a-hotel-descriptive-content-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-2020a-hotel-descriptive-content-resource-defs-openapi.json
- filename: opentravel-2020a-facility-resource-defs-openapi.json
  format: json
  label: OpenTravel 2020A Facility Resource
  slug: opentravel-2020a-facility-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-2020a-facility-resource-defs-openapi.json
- filename: opentravel-2018a-hospitality-offers-resource-defs-openapi.json
  format: json
  label: OpenTravel 2018A Hospitality Offers Resource
  slug: opentravel-2018a-hospitality-offers-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-2018a-hospitality-offers-resource-defs-openapi.json
- filename: opentravel-2018a-facility-resource-defs-openapi.json
  format: json
  label: OpenTravel 2018A Facility Resource
  slug: opentravel-2018a-facility-resource
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/openapi/opentravel-2018a-facility-resource-defs-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opentravel.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: opentraveldevelopersnetwork.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: opentravelmodel.net
  spf: true
  spf_record: v=spf1 ip4:3.135.211.37 +a +mx ~all
hosts:
- cert_expires: Sep  9 21:25:29 2026 GMT
  host: opentravel.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  role: main website, MCP server, OAuth 2.1 authorization server
  tls_version: TLSv1.3
- cert_expires: Sep 21 08:46:49 2026 GMT
  cert_issuer: Let's Encrypt (CN=YR1)
  host: www.opentraveldevelopersnetwork.com
  hsts: false
  https: true
  role: OpenTravel Developers Network (ODN) developer portal
  tls_version: TLSv1.3
- cert_expires: Oct 17 16:01:04 2026 GMT
  cert_issuer: GlobalSign GCC R6 AlphaSSL CA 2025
  host: opentravelmodel.net
  hsts: false
  https: true
  role: OTM Library Repository console
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
  note: 'Not a real host. Six of the eight published documents declare host 127.0.0.1 and two declare example.com, and every one declares `schemes: [http]`. Implementers must supply their own host and serve over HTTPS; the artifact does not say so.'
  role: placeholder host declared by the published Swagger 2.0 contracts
kind: domain-security
layout: security
method: probed
name: Opentravel Alliance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenTravel Alliance, probed live across 4 host(s) and 3 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenTravel Alliance
provider_slug: opentravel-alliance
slug: opentravel-alliance-domain-security
source_filename: opentravel-alliance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of every apis.yml host and every OpenAPI servers[] host\n  (0-working/probe-domain-security.py, plus manual openssl/dig probes of the two OpenTravel-run\n  service hosts the automated pass did not reach)\nhosts:\n- host: opentravel.org\n  role: main website, MCP server, OAuth 2.1 authorization server\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 21:25:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.opentraveldevelopersnetwork.com\n  role: OpenTravel Developers Network (ODN) developer portal\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: \"Let's Encrypt (CN=YR1)\"\n  cert_expires: Sep 21 08:46:49 2026 GMT\n  hsts: false\n- host: opentravelmodel.net\n  role: OTM Library Repository console\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: GlobalSign GCC R6 AlphaSSL CA 2025\n  cert_expires: Oct 17 16:01:04 2026 GMT\n  hsts: false\n- host: 127.0.0.1\n  role:\
  \ placeholder host declared by the published Swagger 2.0 contracts\n  https: false\n  note: >-\n    Not a real host. Six of the eight published documents declare host 127.0.0.1 and two declare\n    example.com, and every one declares `schemes: [http]`. Implementers must supply their own\n    host and serve over HTTPS; the artifact does not say so.\ndomains:\n- domain: opentravel.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: opentraveldevelopersnetwork.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: opentravelmodel.net\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 ip4:3.135.211.37 +a +mx ~all'\n  dmarc: false\nobservations:\n- >-\n  All three OpenTravel-operated hosts negotiate TLS 1.3 with valid certificates.\n- >-\n  HSTS is set only on opentravel.org (max-age 63072000, two years). Neither the developer portal\n  nor the OTM repository console — both of which take a username and password — sends it.\n- >-\n  No domain\
  \ publishes DNSSEC or a CAA record.\n- >-\n  No domain publishes DMARC, so there is no policy on mail spoofing opentravel.org,\n  opentraveldevelopersnetwork.com or opentravelmodel.net. opentravel.org and opentravelmodel.net\n  publish SPF; opentraveldevelopersnetwork.com publishes neither.\nvulnerability_disclosure:\n  published: false\n  probed: '2026-07-28'\n  detail: >-\n    No vulnerability disclosure program and no trust center exist. /.well-known/security.txt\n    returns a real nginx 404 on both opentravel.org and opentraveldevelopersnetwork.com.\n    /security/, /responsible-disclosure/, /vulnerability-disclosure/, /trust/ and /compliance/\n    on opentravel.org all return the WordPress soft-404 homepage (identical 190,291-byte body,\n    zero disclosure or certification keywords). trust.opentravel.org and security.opentravel.org\n    do not resolve. No HackerOne, Bugcrowd or Intigriti program was found. No SOC 2, ISO 27001,\n    PCI DSS, HIPAA or FedRAMP claim appears anywhere\
  \ on the site. Recorded as a verified\n    negative — no security/ vulnerability-disclosure or trust-center artifact was written,\n    because there is nothing to record.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opentravel-alliance/refs/heads/main/security/opentravel-alliance-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Travel
- United States
- Standards
- Aviation
- Hospitality
- Hotels
- Car Rental
- Rail
- Cruise
- Distribution
- GDS
- Booking
- Channel
- XML
- JSON Schema
---
