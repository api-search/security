---
api_specs:
- filename: bizapi-business-intelligence-api-openapi.yml
  format: yaml
  label: BizAPI Business Intelligence API
  slug: bizapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bizapi/refs/heads/main/openapi/bizapi-business-intelligence-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  dmarc: false
  dnssec: false
  domain: naics.com
  spf: true
hosts:
- cert_expires: Sep 27 04:29:38 2026 GMT
  host: www.naics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bizapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BizAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BizAPI
provider_slug: bizapi
slug: bizapi-domain-security
source_filename: bizapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.naics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 04:29:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: naics.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bizapi/refs/heads/main/security/bizapi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Business Intelligence
- Company Data
- CRM
- Firmographic Data
- NAICS
- SIC
---
