---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: talktogina.ai
  spf: false
hosts:
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: talktogina.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Talk To Gina Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Talk To Gina, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Talk To Gina
provider_slug: talktogina-ai
slug: talktogina-ai-domain-security
source_filename: talktogina-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: talktogina.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: talktogina.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/talktogina-ai/security/talktogina-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Automation
- Business
- Productivity
- SaaS
---
