---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: luckmeai.com
  spf: true
hosts:
- cert_expires: Jan 30 05:54:44 2027 GMT
  host: luckmeai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: luckmeai-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for luckmeai-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: luckmeai-com
provider_slug: luckmeai-com
slug: luckmeai-com-domain-security
source_filename: luckmeai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: luckmeai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 05:54:44 2027 GMT\n  hsts: null\ndomains:\n- domain: luckmeai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/luckmeai-com/security/luckmeai-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
