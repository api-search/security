---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: boweryvaluation.com
  spf: true
hosts:
- cert_expires: Sep 30 00:38:50 2026 GMT
  host: www.boweryvaluation.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bowery Valuation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bowery Valuation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bowery Valuation
provider_slug: bowery-valuation
slug: bowery-valuation-domain-security
source_filename: bowery-valuation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boweryvaluation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 00:38:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: boweryvaluation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bowery-valuation/refs/heads/main/security/bowery-valuation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real-Estate
- Commercial Real Estate
- Appraisal
- Valuation
- Property Data
- PropTech
- Lending
---
