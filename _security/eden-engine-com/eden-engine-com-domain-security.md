---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eden-engine.com
  spf: false
hosts:
- cert_expires: Dec 25 14:46:52 2026 GMT
  host: eden-engine.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eden Engine Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eden Engine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Eden Engine
provider_slug: eden-engine-com
slug: eden-engine-com-domain-security
source_filename: eden-engine-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eden-engine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 14:46:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eden-engine.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/eden-engine-com/security/eden-engine-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Assistant
- Productivity
- Software-as-a-Service
- Company
---
