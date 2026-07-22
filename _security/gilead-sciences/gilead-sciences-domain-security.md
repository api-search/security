---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: gilead.com
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.gilead.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Gilead Sciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gilead Sciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Gilead Sciences
provider_slug: gilead-sciences
slug: gilead-sciences-domain-security
source_filename: gilead-sciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gilead.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: gilead.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gilead-sciences/refs/heads/main/security/gilead-sciences-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Pharmaceuticals
- Biotechnology
- Healthcare
- Fortune 500
---
