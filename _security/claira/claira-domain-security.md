---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: claira.io
  spf: true
hosts:
- cert_expires: Jan  3 11:22:51 2027 GMT
  host: www.claira.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Claira Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Claira, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Claira
provider_slug: claira
slug: claira-domain-security
source_filename: claira-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.claira.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 11:22:51 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: claira.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claira/refs/heads/main/security/claira-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Finance
- PrivateMarkets
- DealManagement
- NewYork
---
