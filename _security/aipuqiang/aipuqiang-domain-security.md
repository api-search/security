---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_note: No _dmarc TXT record published for aptr.com.cn at probe time.
  dnssec: false
  domain: aptr.com.cn
  spf: true
hosts:
- cert_expires: Sep 27 01:11:38 2026 GMT
  cert_expiry_note: TLS certificate expires 2026-09-27, thirteen days after this probe (2026-09-14).
  host: aptr.com.cn
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_note: 'The automated probe recorded hsts: null because aptr.com.cn intermittently drops TLS connections behind its Yundun WAF. A manual HEAD on https://aptr.com.cn/ (HTTP/2 200) returned `strict-transport-security: max-age=63072000; includeSubdomains; preload`, so the header is corrected here from that observation.'
  hsts_preload: true
  https: true
  security_headers:
    content_security_policy: frame-ancestors 'self'
    permissions_policy: camera=(), microphone=()
    referrer_policy: strict-origin-when-cross-origin
    x_content_type_options: nosniff
    x_frame_options: SAMEORIGIN
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aipuqiang Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aipuqiang, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aipuqiang
provider_slug: aipuqiang
slug: aipuqiang-domain-security
source_filename: aipuqiang-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aptr.com.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 01:11:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  hsts_note: >-\n    The automated probe recorded hsts: null because aptr.com.cn intermittently drops TLS\n    connections behind its Yundun WAF. A manual HEAD on https://aptr.com.cn/ (HTTP/2 200)\n    returned `strict-transport-security: max-age=63072000; includeSubdomains; preload`,\n    so the header is corrected here from that observation.\n  security_headers:\n    x_frame_options: SAMEORIGIN\n    content_security_policy: frame-ancestors 'self'\n    x_content_type_options: nosniff\n    referrer_policy: strict-origin-when-cross-origin\n    permissions_policy: camera=(), microphone=()\n  cert_expiry_note: >-\n    TLS certificate expires 2026-09-27, thirteen days after this\
  \ probe (2026-09-14).\ndomains:\n- domain: aptr.com.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dmarc_note: No _dmarc TXT record published for aptr.com.cn at probe time.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aipuqiang/refs/heads/main/security/aipuqiang-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Medical Devices
- Healthcare
- Proton Therapy
- Radiation Oncology
- Particle Accelerators
- Medical Equipment
- Oncology
- Manufacturing
- China
---
