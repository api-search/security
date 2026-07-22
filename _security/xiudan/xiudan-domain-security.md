---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: xiudan.net
  spf: true
hosts:
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: xiudan.net
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Xiudan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xiudan (Showball), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Xiudan (Showball)
provider_slug: xiudan
slug: xiudan-domain-security
source_filename: xiudan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xiudan.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: xiudan.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xiudan/refs/heads/main/security/xiudan-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Company
- Social
- Avatars
- Virtual Worlds
- Mobile Apps
- Metaverse
- China
---
