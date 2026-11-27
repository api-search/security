---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: sumibako.com
  spf: true
hosts:
- cert_expires: Feb  1 02:50:15 2027 GMT
  host: sumibako.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sumibako Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sumibako, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sumibako
provider_slug: sumibako-com
slug: sumibako-com-domain-security
source_filename: sumibako-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sumibako.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 02:50:15 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sumibako.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/sumibako-com/security/sumibako-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Note-taking
- Collaboration
- Privacy
- Free-tier
---
