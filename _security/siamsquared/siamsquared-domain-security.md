---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stockradars.co
  spf: true
hosts:
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: stockradars.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Siamsquared Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SiamSquared, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SiamSquared
provider_slug: siamsquared
slug: siamsquared-domain-security
source_filename: siamsquared-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stockradars.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: stockradars.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siamsquared/refs/heads/main/security/siamsquared-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Stocks
- Investing
- Stock Analysis
- Financial Data
- Thailand
- Mobile App
---
