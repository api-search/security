---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: acquislaw.com
  spf: true
hosts:
- cert_expires: Jan  6 23:07:11 2027 GMT
  host: acquislaw.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Acquis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acquis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Acquis
provider_slug: acquislaw-com
slug: acquislaw-com-domain-security
source_filename: acquislaw-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acquislaw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:07:11 2027 GMT\n  hsts: false\ndomains:\n- domain: acquislaw.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/acquislaw-com/security/acquislaw-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Legal Tech
- EU Law
- Software-as-a-Service
---
