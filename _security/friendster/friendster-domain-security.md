---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: friendster.com
  spf: false
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: friendster.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Friendster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Friendster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Friendster
provider_slug: friendster
slug: friendster-domain-security
source_filename: friendster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: friendster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: friendster.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/friendster/refs/heads/main/security/friendster-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Social Network
- Social Media
- Consumer
- Mobile
- Privacy
---
