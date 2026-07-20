---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wangdian.cn
  spf: true
hosts:
- cert_expires: Dec 10 01:34:36 2026 GMT
  host: www.wangdian.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 01:34:36 2026 GMT
  host: open.wangdian.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 10 01:34:36 2026 GMT
  host: api.wangdian.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Huice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Huice, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Huice
provider_slug: huice
slug: huice-domain-security
source_filename: huice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wangdian.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 01:34:36 2026 GMT\n  hsts: false\n- host: open.wangdian.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 10 01:34:36 2026 GMT\n  hsts: false\n- host: api.wangdian.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 10 01:34:36 2026 GMT\n  hsts: false\ndomains:\n- domain: wangdian.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huice/refs/heads/main/security/huice-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- E-commerce
- ERP
- Order Management
- Inventory Management
- Warehouse Management
- Retail
- SaaS
- China
---
