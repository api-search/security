---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brandct.cn
  spf: false
hosts:
- cert_expires: Aug 26 15:03:36 2026 GMT
  host: brandct.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Brandct Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BrandCT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: BrandCT
provider_slug: brandct
slug: brandct-domain-security
source_filename: brandct-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brandct.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 26 15:03:36 2026 GMT\n  hsts: false\ndomains:\n- domain: brandct.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandct/refs/heads/main/security/brandct-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Enterprise
- Retail
- Market Research
- Retail Analytics
- Point of Sale
- Consumer Packaged Goods
- China
---
