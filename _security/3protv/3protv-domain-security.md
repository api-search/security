---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 3protv.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: 3protv.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 3Protv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3ProTV, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 3ProTV
provider_slug: 3protv
slug: 3protv-domain-security
source_filename: 3protv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 3protv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: 3protv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3protv/refs/heads/main/security/3protv-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Media
- Financial Media
- Video
- Streaming
- Subscription
- Education
- South Korea
- Content
---
