---
api_specs:
- filename: claude-world-com-openapi-generated.yml
  format: yaml
  label: ClaudeWorld API
  slug: claude-world-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claude-world-com/openapi/_ae-authored/claude-world-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: claude-world.com
  spf: true
hosts:
- cert_expires: Jan  4 22:14:44 2027 GMT
  host: claude-world.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Claude World Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClaudeWorld, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: ClaudeWorld
provider_slug: claude-world-com
slug: claude-world-com-domain-security
source_filename: claude-world-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: claude-world.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 22:14:44 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: claude-world.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/claude-world-com/security/claude-world-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Developer Tools
- Documentation
- Open Source
- Community
---
