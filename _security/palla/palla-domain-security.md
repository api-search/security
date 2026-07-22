---
api_specs:
- filename: palla-platform-openapi.yml
  format: yaml
  label: Palla Platform Partner API
  slug: palla-platform-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palla/refs/heads/main/openapi/palla-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: palla.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: palla.app
  spf: true
hosts:
- cert_expires: Oct  7 16:57:50 2026 GMT
  host: www.palla.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: api.platform.palla.app
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Palla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Palla, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Palla
provider_slug: palla
slug: palla-domain-security
source_filename: palla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.palla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 16:57:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.platform.palla.app\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: palla.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: palla.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/palla/refs/heads/main/security/palla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Cross-Border Payments
- Remittances
- P2P Payments
- Money Transfer
- Embedded Finance
---
