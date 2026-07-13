---
api_specs:
- filename: fis-payments-openapi.yml
  format: yaml
  label: FIS Payments API
  slug: fis-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-payments-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "visa.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fisglobal.com
  spf: true
hosts:
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: codeconnect.fisglobal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.fisglobal.com
  https: false
- host: sandbox.api.fisglobal.com
  https: false
kind: domain-security
layout: security
method: probed
name: Fis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FIS Global, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FIS Global
provider_slug: fis
slug: fis-domain-security
source_filename: fis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codeconnect.fisglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fisglobal.com\n  https: false\n- host: sandbox.api.fisglobal.com\n  https: false\ndomains:\n- domain: fisglobal.com\n  dnssec: false\n  caa:\n  - 0 issue \"visa.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/security/fis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Core Banking
- Financial Services
- Payments
- Fintech
---
