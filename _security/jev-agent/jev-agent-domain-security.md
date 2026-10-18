---
api_specs:
- filename: jev-agent-openapi-generated.yml
  format: yaml
  label: Jev Agent (Jagent) API
  slug: jev-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jev-agent/refs/heads/main/openapi/_ae-authored/jev-agent-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jev-agent.com
  spf: true
hosts:
- cert_expires: Dec 17 08:13:20 2026 GMT
  host: jev-agent.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jev Agent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jev Agent (Jagent), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jev Agent (Jagent)
provider_slug: jev-agent
slug: jev-agent-domain-security
source_filename: jev-agent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jev-agent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 08:13:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jev-agent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jev-agent/refs/heads/main/security/jev-agent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI API
- Classification
- Token Billing
- Developer Tools
---
