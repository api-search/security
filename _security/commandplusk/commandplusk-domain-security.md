---
api_specs:
- filename: commandplusk-openapi-generated.yml
  format: yaml
  label: CMD+K API
  slug: commandplusk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commandplusk/refs/heads/main/openapi/_ae-authored/commandplusk-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: commandplusk.com
  spf: false
hosts:
- cert_expires: Dec 13 16:58:58 2026 GMT
  host: commandplusk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Commandplusk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CMD+K, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: CMD+K
provider_slug: commandplusk
slug: commandplusk-domain-security
source_filename: commandplusk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: commandplusk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 16:58:58 2026 GMT\n  hsts: false\ndomains:\n- domain: commandplusk.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commandplusk/refs/heads/main/security/commandplusk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Assistant
- Platform
- SaaS
- Developer
---
