---
api_specs:
- filename: symphonyos-openapi-generated.yml
  format: yaml
  label: SymphonyOS API
  slug: symphonyos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphonyos/refs/heads/main/openapi/_ae-authored/symphonyos-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: symphonyos.co
  spf: true
hosts:
- cert_expires: Dec 27 22:35:21 2026 GMT
  host: symphonyos.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Symphonyos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SymphonyOS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SymphonyOS
provider_slug: symphonyos
slug: symphonyos-domain-security
source_filename: symphonyos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: symphonyos.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 22:35:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: symphonyos.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symphonyos/refs/heads/main/security/symphonyos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Music
- Platform
- Agents
---
