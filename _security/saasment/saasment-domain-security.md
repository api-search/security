---
api_specs:
- filename: saasment-openapi.yml
  format: yaml
  label: Saasment API
  slug: saasment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saasment/refs/heads/main/openapi/saasment-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: saasment.com
  spf: false
hosts:
- cert_expires: Oct  6 08:02:21 2026 GMT
  host: www.saasment.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.saasment.com
  https: false
kind: domain-security
layout: security
method: probed
name: Saasment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saasment, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Saasment
provider_slug: saasment
slug: saasment-domain-security
source_filename: saasment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saasment.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:02:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.saasment.com\n  https: false\ndomains:\n- domain: saasment.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saasment/refs/heads/main/security/saasment-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SaaS Security
- SSPM
- Cloud Security
- Cost Optimization
- Compliance
- Misconfigurations
---
