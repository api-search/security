---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dispatchgoods.com
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: dispatchgoods.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dispatch Goods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dispatch Goods, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Dispatch Goods
provider_slug: dispatch-goods
slug: dispatch-goods-domain-security
source_filename: dispatch-goods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dispatchgoods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: dispatchgoods.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dispatch-goods/refs/heads/main/security/dispatch-goods-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Reusable Packaging
- Sustainability
- Reverse Logistics
- Food Delivery
- Circular Economy
---
