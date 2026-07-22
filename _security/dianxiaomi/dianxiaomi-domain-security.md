---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dianxiaomi.com
  spf: true
hosts:
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: www.dianxiaomi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dianxiaomi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dianxiaomi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dianxiaomi
provider_slug: dianxiaomi
slug: dianxiaomi-domain-security
source_filename: dianxiaomi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dianxiaomi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: dianxiaomi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dianxiaomi/refs/heads/main/security/dianxiaomi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- E-commerce
- ERP
- Cross-Border
- Logistics
- Order Management
- Inventory
- SaaS
---
