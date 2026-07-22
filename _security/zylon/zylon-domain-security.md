---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zylon.ai
  spf: true
hosts:
- cert_expires: Sep 18 19:26:16 2026 GMT
  host: zylon.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zylon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zylon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zylon
provider_slug: zylon
slug: zylon-domain-security
source_filename: zylon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zylon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 19:26:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zylon.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zylon/refs/heads/main/security/zylon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
