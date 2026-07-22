---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: igetget.com
  spf: true
hosts:
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: igetget.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Igetget Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for igetget, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: igetget
provider_slug: igetget
slug: igetget-domain-security
source_filename: igetget-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: igetget.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: igetget.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/igetget/refs/heads/main/security/igetget-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Knowledge
- Education
- E-Learning
- Audiobooks
- Content
- Mobile App
- China
---
