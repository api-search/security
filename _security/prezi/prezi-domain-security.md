---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: prezi.com
  spf: true
hosts:
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: www.prezi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Prezi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prezi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Prezi
provider_slug: prezi
slug: prezi-domain-security
source_filename: prezi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prezi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: prezi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prezi/refs/heads/main/security/prezi-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Consumer
- Presentations
- Productivity
- SaaS
- Content Creation
- Design
- Video
---
