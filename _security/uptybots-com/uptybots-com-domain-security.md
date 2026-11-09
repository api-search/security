---
api_specs:
- filename: uptybots-com-openapi-generated.yml
  format: yaml
  label: uptybots-com API
  slug: uptybots-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptybots-com/openapi/_ae-authored/uptybots-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uptybots.com
  spf: true
hosts:
- cert_expires: Dec 20 15:28:03 2026 GMT
  host: uptybots.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Uptybots Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for uptybots-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: uptybots-com
provider_slug: uptybots-com
slug: uptybots-com-domain-security
source_filename: uptybots-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uptybots.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 15:28:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uptybots.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/uptybots-com/security/uptybots-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Monitoring
- Uptime
- Artificial Intelligence
- MCP
---
