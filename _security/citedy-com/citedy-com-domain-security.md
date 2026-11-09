---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: citedy.com
  spf: true
hosts:
- cert_expires: Jan 30 21:50:59 2027 GMT
  host: citedy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Citedy Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citedy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Citedy
provider_slug: citedy-com
slug: citedy-com-domain-security
source_filename: citedy-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: citedy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 21:50:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: citedy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/citedy-com/security/citedy-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- SEO
- Content Automation
- Agents
- Platform
---
