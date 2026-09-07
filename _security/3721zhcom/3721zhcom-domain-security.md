---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 3721zh.com
  spf: true
hosts:
- cert_expires: Nov  1 09:32:24 2026 GMT
  host: www.3721zh.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 3721Zhcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3721zh.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 3721zh.com
provider_slug: 3721zhcom
slug: 3721zhcom-domain-security
source_filename: 3721zhcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.3721zh.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  1 09:32:24 2026 GMT\n  hsts: false\ndomains:\n- domain: 3721zh.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3721zhcom/refs/heads/main/security/3721zhcom-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- E-Commerce
- Retail
- SaaS
- Marketing
- Loyalty
- Supply Chain
- Food and Beverage
- Local Commerce
- Private Domain Traffic
- WeChat Mini Programs
- China
---
