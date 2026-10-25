---
api_specs:
- filename: amber-electric-amber-api-openapi.yml
  format: yaml
  label: Amber Electric Amber API
  slug: amber-electric-amber-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amber-electric/refs/heads/main/openapi/amber-electric-amber-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazontrust.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amber.com.au
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cdr.gov.au
  spf: true
hosts:
- cert_expires: Dec 14 11:30:16 2026 GMT
  host: amber.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 18:53:49 2027 GMT
  host: www.cdr.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 02:22:51 2026 GMT
  host: public.cdr.amber.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Amber Electric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amber Electric, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amber Electric
provider_slug: amber-electric
slug: amber-electric-domain-security
source_filename: amber-electric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amber.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 11:30:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.cdr.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 18:53:49 2027 GMT\n  hsts: null\n- host: public.cdr.amber.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 02:22:51 2026 GMT\n  hsts: null\ndomains:\n- domain: amber.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cdr.gov.au\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amber-electric/refs/heads/main/security/amber-electric-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
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
