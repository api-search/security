---
api_specs:
- filename: modusbox-orca-contract-notice.yml
  format: yaml
  label: PortX ORCA (Open Reusable Core API)
  slug: portx-orca-open-reusable-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modusbox/refs/heads/main/openapi/modusbox-orca-contract-notice.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: portx.io
  spf: true
hosts:
- cert_expires: Oct  3 15:04:00 2026 GMT
  host: portx.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 06:25:18 2026 GMT
  host: orca-docs.portx.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- host: api.portx.io
  https: false
kind: domain-security
layout: security
method: probed
name: Modusbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ModusBox, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ModusBox
provider_slug: modusbox
slug: modusbox-domain-security
source_filename: modusbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:04:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: orca-docs.portx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 06:25:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.portx.io\n  https: false\ndomains:\n- domain: portx.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modusbox/refs/heads/main/security/modusbox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Banking
- Core Banking
- Credit Unions
- Financial Services
- Integration
- iPaaS
- Payments
- ISO 20022
- Open Banking
- Data
---
