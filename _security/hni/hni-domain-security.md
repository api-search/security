---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hni.com
  spf: true
hosts:
- cert_expires: Sep 14 03:11:15 2026 GMT
  host: www.hni.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hni, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: hni
provider_slug: hni
slug: hni-domain-security
source_filename: hni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:11:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hni.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hni/refs/heads/main/security/hni-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 1000
---
