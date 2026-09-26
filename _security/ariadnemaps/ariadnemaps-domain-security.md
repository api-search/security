---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ariadne.inc
  spf: true
hosts:
- cert_expires: Nov 26 05:48:25 2026 GMT
  host: www.ariadne.inc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ariadnemaps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ariadnemaps, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ariadnemaps
provider_slug: ariadnemaps
slug: ariadnemaps-domain-security
source_filename: ariadnemaps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ariadne.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 05:48:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ariadne.inc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ariadnemaps/refs/heads/main/security/ariadnemaps-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- PeopleCounting
- PrivacyFirst
- IoT
- Analytics
---
