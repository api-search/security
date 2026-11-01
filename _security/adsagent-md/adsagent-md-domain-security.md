---
api_specs:
- filename: adsagent-md-openapi-generated.yml
  format: yaml
  label: adsagent-md API
  slug: adsagent-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsagent-md/openapi/_ae-authored/adsagent-md-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adsagent.md
  spf: true
hosts:
- cert_expires: Dec  2 16:41:42 2026 GMT
  host: adsagent.md
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adsagent Md Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for adsagent-md, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: adsagent-md
provider_slug: adsagent-md
slug: adsagent-md-domain-security
source_filename: adsagent-md-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adsagent.md\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 16:41:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adsagent.md\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/adsagent-md/security/adsagent-md-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AdTech
- Marketing Automation
- AI
- MCP
---
