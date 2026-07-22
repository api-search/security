---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: veluga.kr
  spf: true
hosts:
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: business.veluga.kr
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Veluga Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veluga, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Veluga
provider_slug: veluga
slug: veluga-domain-security
source_filename: veluga-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: business.veluga.kr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: veluga.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veluga/refs/heads/main/security/veluga-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Alcohol
- Beverage
- Wholesale
- Marketplace
- B2B
- Distribution
- E-Commerce
- South Korea
---
