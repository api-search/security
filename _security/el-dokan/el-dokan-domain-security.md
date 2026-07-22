---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: el-dokan.com
  spf: true
hosts:
- cert_expires: Aug 17 14:46:44 2026 GMT
  host: el-dokan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: El Dokan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for El-Dokan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: El-Dokan
provider_slug: el-dokan
slug: el-dokan-domain-security
source_filename: el-dokan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: el-dokan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 14:46:44 2026 GMT\n  hsts: false\ndomains:\n- domain: el-dokan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/el-dokan/refs/heads/main/security/el-dokan-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- eCommerce
- Headless Commerce
- Composable Commerce
- RetailTech
- API-First
- SaaS
- Multi-Vendor Marketplace
- MENA
- Egypt
---
