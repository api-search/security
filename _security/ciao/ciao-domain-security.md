---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: meetciao.com
  spf: true
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: meetciao.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ciao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ciao, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ciao
provider_slug: ciao
slug: ciao-domain-security
source_filename: ciao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meetciao.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: meetciao.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ciao/refs/heads/main/security/ciao-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Home Sharing
- Hospitality
- Community
- Marketplace
- Consumer
- Seedcamp
---
