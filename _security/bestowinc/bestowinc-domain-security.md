---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bestowinc.com
  spf: true
hosts:
- cert_expires: Jan 31 16:51:21 2027 GMT
  host: bestowinc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bestowinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bestowinc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bestowinc
provider_slug: bestowinc
slug: bestowinc-domain-security
source_filename: bestowinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bestowinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 16:51:21 2027 GMT\n  hsts: false\ndomains:\n- domain: bestowinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bestowinc/refs/heads/main/security/bestowinc-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- Employee Rewards
- Gift Cards
---
