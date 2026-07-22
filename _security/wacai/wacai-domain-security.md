---
description: ''
domains:
- caa:
  - qsh2-idc.wacai.com.
  dmarc: false
  dnssec: true
  domain: wacai.com
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: wacai.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Wacai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for wacai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: wacai
provider_slug: wacai
slug: wacai-domain-security
source_filename: wacai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wacai.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: wacai.com\n  dnssec: true\n  caa:\n  - qsh2-idc.wacai.com.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wacai/refs/heads/main/security/wacai-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Company
- Fintech
- Personal Finance
- Accounting
- Wealth Management
- Open Platform
- API Gateway
- China
---
