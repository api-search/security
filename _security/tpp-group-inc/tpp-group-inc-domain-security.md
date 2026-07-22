---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tppgroup.co
  spf: true
hosts:
- cert_expires: Oct  1 17:25:58 2026 GMT
  host: tppgroup.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tpp Group Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TPP GROUP INC., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TPP GROUP INC.
provider_slug: tpp-group-inc
slug: tpp-group-inc-domain-security
source_filename: tpp-group-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tppgroup.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 17:25:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tppgroup.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tpp-group-inc/refs/heads/main/security/tpp-group-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- Media Intelligence
- Arabic Content
- Advertising
- Audience Analytics
- Podcasts
- Content Production
---
