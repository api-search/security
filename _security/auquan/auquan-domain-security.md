---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: auquan.com
  spf: true
hosts:
- cert_expires: Aug 24 06:17:49 2026 GMT
  host: auquan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Auquan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auquan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Auquan
provider_slug: auquan
slug: auquan-domain-security
source_filename: auquan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auquan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 06:17:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: auquan.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auquan/refs/heads/main/security/auquan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Agentic AI
- Financial Services
- Fintech
- Data Analytics
- Machine Learning
---
