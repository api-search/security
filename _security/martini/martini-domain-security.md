---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: martini.film
  spf: true
hosts:
- cert_expires: Oct 12 13:01:41 2026 GMT
  host: www.martini.film
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Martini Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Martini, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Martini
provider_slug: martini
slug: martini-domain-security
source_filename: martini-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.martini.film\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 13:01:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: martini.film\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/martini/refs/heads/main/security/martini-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Video
- Filmmaking
- Generative AI
- Creative Tools
- Model Context Protocol
- Agents
- Collaboration
- Media Production
---
