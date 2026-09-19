---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aikenong.com.cn
  spf: false
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.aikenong.com.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aikenong Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aikenong, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Aikenong
provider_slug: aikenong
slug: aikenong-domain-security
source_filename: aikenong-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aikenong.com.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: aikenong.com.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aikenong/refs/heads/main/security/aikenong-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Agriculture
- AgTech
- Smart Agriculture
- Artificial Intelligence
- Remote Sensing
- IoT
- Data & Analytics
- China
---
