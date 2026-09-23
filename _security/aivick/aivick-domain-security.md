---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aivick.co.jp
  spf: true
hosts:
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: aivick.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aivick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aivick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aivick
provider_slug: aivick
slug: aivick-domain-security
source_filename: aivick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aivick.co.jp\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: aivick.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aivick/refs/heads/main/security/aivick-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Food Tech
- Health
- ICT
- Wellness
---
