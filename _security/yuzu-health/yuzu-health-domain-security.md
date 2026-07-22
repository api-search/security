---
api_specs:
- filename: yuzu-health-openapi-original.json
  format: json
  label: Yuzu API
  slug: yuzu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: yuzu.health
  spf: true
hosts:
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: yuzu.health
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yuzu Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yuzu Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Yuzu Health
provider_slug: yuzu-health
slug: yuzu-health-domain-security
source_filename: yuzu-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yuzu.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yuzu.health\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/security/yuzu-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health
- Healthcare
- Insurance
- Health Plans
- Benefits Administration
- Claims
- Enrollment
- Payers
- Self-Funded
---
