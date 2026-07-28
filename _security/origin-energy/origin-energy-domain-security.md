---
api_specs:
- filename: consumer-data-standards-energy-api-openapi.json
  format: json
  label: Origin Energy CDR Energy API
  slug: origin-energy-cdr-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-energy/refs/heads/main/openapi/consumer-data-standards-energy-api-openapi.json
- filename: consumer-data-standards-common-api-openapi.json
  format: json
  label: Origin Energy CDR Public Discovery API
  slug: origin-energy-cdr-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-energy/refs/heads/main/openapi/consumer-data-standards-common-api-openapi.json
- filename: consumer-data-standards-energy-api-openapi.json
  format: json
  label: Origin Energy Plan Reference Data API (AER Energy Made Easy)
  slug: origin-energy-plan-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-energy/refs/heads/main/openapi/consumer-data-standards-energy-api-openapi.json
- filename: origin-energy-kraken-default-openapi.yml
  format: yaml
  label: Origin Energy Kraken REST API
  slug: origin-energy-kraken-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-energy/refs/heads/main/openapi/origin-energy-kraken-default-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: originenergy.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: origin-kraken.energy
  spf: true
  spf_record: v=spf1 -all
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: www.originenergy.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.mydata.cdr.originenergy.com.au
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate in certificate chain (_ssl.c:1082)'
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: public.mydata.cdr.originenergy.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api.origin-kraken.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: auth.origin-kraken.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: developer.origin-kraken.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Origin Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Origin Energy, probed live across 6 host(s) and 2 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Origin Energy
provider_slug: origin-energy
slug: origin-energy-domain-security
source_filename: origin-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts, extended 2026-07-27 with the origin-kraken.energy\n  platform hosts\nhosts:\n- host: www.originenergy.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: null\n- host: api.mydata.cdr.originenergy.com.au\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    in certificate chain (_ssl.c:1082)'\n  hsts: null\n- host: public.mydata.cdr.originenergy.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\n- host: api.origin-kraken.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: auth.origin-kraken.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.origin-kraken.energy\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: originenergy.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: origin-kraken.energy\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 -all\n  dmarc: true\n  dmarc_policy: reject\nnotes:\n- 'api.mydata.cdr.originenergy.com.au fails public certificate verification by design: its chain terminates\n  at the ACCC''s private CDR Root CA, not a public trust anchor. That is the Consumer Data Right PKI working,\n  not a misconfiguration.'\n- No HSTS on any originenergy.com.au host; all three origin-kraken.energy hosts set max-age=31536000.\n- originenergy.com.au publishes CAA (pki.goog, ssl.com, Amazon wildcards);\
  \ origin-kraken.energy publishes\n  none.\n- Neither domain is DNSSEC signed.\n- origin-kraken.energy publishes v=spf1 -all (send-nothing) and DMARC p=reject.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/origin-energy/refs/heads/main/security/origin-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retail
- Consumer Data Right
- Smart Metering
- Solar
- DER
- Demand Response
- Energy Markets
---
