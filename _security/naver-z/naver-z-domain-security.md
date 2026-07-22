---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: naverz-corp.com
  spf: true
hosts:
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: naverz-corp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Naver Z Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NAVER Z, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NAVER Z
provider_slug: naver-z
slug: naver-z-domain-security
source_filename: naver-z-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: naverz-corp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: naverz-corp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/naver-z/refs/heads/main/security/naver-z-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Metaverse
- Avatar
- Social
- Gaming
- Mobile
- Developer Tools
- SDK
- Scripting
---
