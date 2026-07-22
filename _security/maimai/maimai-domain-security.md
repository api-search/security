---
description: ''
domains:
- caa:
  - c300578a653f4a50ae4ef806d5cb3630.vip1.huaweicloudwaf.com.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: maimai.cn
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: maimai.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maimai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maimai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Maimai
provider_slug: maimai
slug: maimai-domain-security
source_filename: maimai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maimai.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: maimai.cn\n  dnssec: true\n  caa:\n  - c300578a653f4a50ae4ef806d5cb3630.vip1.huaweicloudwaf.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maimai/refs/heads/main/security/maimai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Professional Networking
- Social Network
- Recruitment
- Careers
- China
---
