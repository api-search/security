---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: finlessfoods.com
  spf: true
hosts:
- cert_expires: Oct 18 22:24:50 2026 GMT
  host: finlessfoods.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finless Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finless Foods, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Finless Foods
provider_slug: finless-foods
slug: finless-foods-domain-security
source_filename: finless-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finlessfoods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 22:24:50 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: finlessfoods.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finless-foods/refs/heads/main/security/finless-foods-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cellular Agriculture
- Cell-Cultured Seafood
- Alternative Protein
- Food Technology
- Biotechnology
- Sustainability
- Consumer Packaged Goods
- United States
---
