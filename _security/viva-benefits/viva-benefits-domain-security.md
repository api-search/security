---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vivabenefits.com
  spf: true
hosts:
- cert_expires: Oct 15 13:03:11 2026 GMT
  host: vivabenefits.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Viva Benefits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Viva Benefits, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Viva Benefits
provider_slug: viva-benefits
slug: viva-benefits-domain-security
source_filename: viva-benefits-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vivabenefits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 13:03:11 2026 GMT\n  hsts: false\ndomains:\n- domain: vivabenefits.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viva-benefits/refs/heads/main/security/viva-benefits-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Benefits
- Equity
- Human Resources
- Compensation
- Fintech
---
