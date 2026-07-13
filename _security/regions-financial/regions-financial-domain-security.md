---
api_specs:
- filename: regions-open-banking-openapi.yml
  format: yaml
  label: Regions Open Banking API
  slug: regions-open-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regions-financial/refs/heads/main/openapi/regions-open-banking-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild ";"
  - 0 iodef "mailto:was@regions.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: regions.com
  spf: true
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: www.regions.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: ir.regions.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.regions.com
  https: false
kind: domain-security
layout: security
method: probed
name: Regions Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for regions-financial, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: regions-financial
provider_slug: regions-financial
slug: regions-financial-domain-security
source_filename: regions-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.regions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\n- host: ir.regions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.regions.com\n  https: false\ndomains:\n- domain: regions.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:was@regions.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regions-financial/refs/heads/main/security/regions-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Financial Services
- Open Banking
- FDX
- Consumer Banking
- Wealth Management
- Fortune 500
---
