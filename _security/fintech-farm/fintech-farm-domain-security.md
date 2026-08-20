---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fintech-farm.com
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: www.fintech-farm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fintech Farm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fintech Farm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fintech Farm
provider_slug: fintech-farm
slug: fintech-farm-domain-security
source_filename: fintech-farm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fintech-farm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: fintech-farm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fintech-farm/refs/heads/main/security/fintech-farm-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Banking
- Financial-Services
- Neobank
- Digital Banking
- Fintech
- Credit
- Emerging Markets
- Banking as a Service
- Mobile Banking
---
