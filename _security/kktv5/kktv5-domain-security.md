---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kktv5.com
  spf: false
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: www.kktv5.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kktv5 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KK直播 (KK Live), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: KK直播 (KK Live)
provider_slug: kktv5
slug: kktv5-domain-security
source_filename: kktv5-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kktv5.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: kktv5.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kktv5/refs/heads/main/security/kktv5-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Live Streaming
- Video
- Social Networking
- Entertainment
- Consumer
- Mobile Applications
- China
---
