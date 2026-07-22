---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: myyellow.com
  spf: true
hosts:
- cert_expires: Sep  2 02:09:49 2026 GMT
  host: www.myyellow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yrc Worldwide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YRC Worldwide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: YRC Worldwide
provider_slug: yrc-worldwide
slug: yrc-worldwide-domain-security
source_filename: yrc-worldwide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.myyellow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 02:09:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: myyellow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yrc-worldwide/refs/heads/main/security/yrc-worldwide-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
---
