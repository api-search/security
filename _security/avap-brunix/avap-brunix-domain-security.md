---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: avapframework.com
  spf: false
hosts:
- cert_expires: Sep  4 17:17:29 2026 GMT
  host: www.avapframework.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Avap Brunix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AVAP BRUNIX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AVAP BRUNIX
provider_slug: avap-brunix
slug: avap-brunix-domain-security
source_filename: avap-brunix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avapframework.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  4 17:17:29 2026 GMT\n  hsts: false\ndomains:\n- domain: avapframework.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avap-brunix/refs/heads/main/security/avap-brunix-domain-security.yml
summary_line: TLSv1.2
tags:
- AI
- API Development
- Developer Tools
- Low Code
- Automation
---
