---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moonchild.ai
  spf: true
hosts:
- cert_expires: Dec 23 14:43:50 2026 GMT
  host: www.moonchild.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Moonchild Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moonchild, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Moonchild
provider_slug: moonchild
slug: moonchild-domain-security
source_filename: moonchild-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moonchild.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 14:43:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: moonchild.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/moonchild/security/moonchild-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Design
- Product
- Collaboration
- Automation
- Platform
---
