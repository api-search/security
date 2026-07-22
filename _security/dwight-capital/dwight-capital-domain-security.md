---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: dwightcapital.com
  spf: false
hosts:
- cert_expires: Sep 20 00:31:37 2026 GMT
  host: www.dwightcapital.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dwight Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dwight Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Dwight Capital
provider_slug: dwight-capital
slug: dwight-capital-domain-security
source_filename: dwight-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dwightcapital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:31:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dwightcapital.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dwight-capital/refs/heads/main/security/dwight-capital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Commercial Real Estate
- Real Estate Finance
- HUD Lending
- FHA Lending
- Bridge Lending
- Multifamily
- Mortgage
- Financial Services
---
