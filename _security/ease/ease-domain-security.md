---
api_specs:
- filename: ease-content-openapi.yml
  format: yaml
  label: Ease Content & Marketplace API
  slug: ease-content-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-content-openapi.yml
- filename: ease-status-openapi.yml
  format: yaml
  label: Ease Status API
  slug: ease-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/openapi/ease-status-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ease.com
  spf: true
hosts:
- cert_expires: Sep 14 21:45:16 2026 GMT
  host: www.ease.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ease Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ease, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ease
provider_slug: ease
slug: ease-domain-security
source_filename: ease-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ease.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 21:45:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ease.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ease/refs/heads/main/security/ease-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United States
- Employee Benefits
- Benefits Administration
- Group Benefits
- Health Insurance
- Insurtech
- Brokers
- Enrollment
- EDI
- Payroll
- Human Resources
- Marketplace
- Status
---
