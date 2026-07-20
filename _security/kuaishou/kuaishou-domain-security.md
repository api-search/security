---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kuaishou.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kwai.com
  spf: true
hosts:
- cert_expires: Sep  7 03:46:08 2026 GMT
  host: www.kuaishou.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  7 03:46:08 2026 GMT
  host: open.kuaishou.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 30 08:23:34 2026 GMT
  host: developers.kwai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kuaishou Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kuaishou, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kuaishou
provider_slug: kuaishou
slug: kuaishou-domain-security
source_filename: kuaishou-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kuaishou.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  7 03:46:08 2026 GMT\n  hsts: false\n- host: open.kuaishou.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  7 03:46:08 2026 GMT\n  hsts: false\n- host: developers.kwai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:23:34 2026 GMT\n  hsts: false\ndomains:\n- domain: kuaishou.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: kwai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kuaishou/refs/heads/main/security/kuaishou-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Consumer
- Social
- Video
- Short Video
- Live Streaming
- Advertising
- Marketing
- Social Media
- Content
- China
---
