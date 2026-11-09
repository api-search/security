---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aethereum.dev
  spf: false
hosts:
- cert_expires: Jan 15 18:09:49 2027 GMT
  host: aethereum.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aethereum Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aethereum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Aethereum
provider_slug: aethereum-dev
slug: aethereum-dev-domain-security
source_filename: aethereum-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aethereum.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 18:09:49 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aethereum.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/aethereum-dev/security/aethereum-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Collaboration
- Coordination
- Development
- Platform
---
