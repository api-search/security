---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: divx.com
  spf: true
hosts:
- cert_expires: Aug 26 14:19:16 2026 GMT
  host: www.divx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Divx Inc Nasdaqgs Divx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DivX, Inc. (NasdaqGS:DIVX), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DivX, Inc. (NasdaqGS:DIVX)
provider_slug: divx-inc-nasdaqgs-divx
slug: divx-inc-nasdaqgs-divx-domain-security
source_filename: divx-inc-nasdaqgs-divx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.divx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 14:19:16 2026 GMT\n  hsts: false\ndomains:\n- domain: divx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/divx-inc-nasdaqgs-divx/refs/heads/main/security/divx-inc-nasdaqgs-divx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Video
- Codec
- Media
- Streaming
- Software
---
