---
description: ''
domains:
- caa:
  - www.tongdun.cn.
  dmarc: false
  dnssec: true
  domain: tongdun.cn
  spf: true
hosts:
- cert_expires: Sep 15 07:31:06 2026 GMT
  host: tongdun.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tongdun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tongdun, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Tongdun
provider_slug: tongdun
slug: tongdun-domain-security
source_filename: tongdun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tongdun.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:31:06 2026 GMT\n  hsts: false\ndomains:\n- domain: tongdun.cn\n  dnssec: true\n  caa:\n  - www.tongdun.cn.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tongdun/refs/heads/main/security/tongdun-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Risk Management
- Fraud Detection
- Anti-Fraud
- Risk Control
- Financial Services
- Credit Risk
- Artificial Intelligence
- Decisioning
- RegTech
- China
---
