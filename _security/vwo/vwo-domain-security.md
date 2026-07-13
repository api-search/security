---
api_specs:
- filename: vwo-openapi.yml
  format: yaml
  label: VWO Data API
  slug: vwo-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vwo/refs/heads/main/openapi/vwo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vwo.com
  spf: true
hosts:
- cert_expires: Oct  4 14:00:41 2026 GMT
  host: vwo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 21:17:14 2026 GMT
  host: developers.vwo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 21:17:14 2026 GMT
  host: app.vwo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vwo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VWO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VWO
provider_slug: vwo
slug: vwo-domain-security
source_filename: vwo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vwo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:00:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.vwo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:17:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.vwo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:17:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vwo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vwo/refs/heads/main/security/vwo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Experimentation
- AB Testing
- Personalization
- Conversion Optimization
- Feature Flags
---
