---
api_specs:
- filename: Encompass_Developer_Connect_postman_collection.json
  format: json
  label: Encompass Developer Connect (sibling product under ICE)
  slug: encompass-developer-connect
  spec_type: Postman
  url: https://help.icemortgagetechnology.com/documentation/developer-connect/postman/Encompass_Developer_Connect_postman_collection.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ice.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: icemortgagetechnology.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: mortgagetech.ice.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 12:47:10 2026 GMT
  host: developer.ice.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:25:55 2026 GMT
  host: developer.icemortgagetechnology.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Black Knight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Black Knight (Acquired by ICE — Now ICE Mortgage Technology), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Black Knight (Acquired by ICE — Now ICE Mortgage Technology)
provider_slug: black-knight
slug: black-knight-domain-security
source_filename: black-knight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mortgagetech.ice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: developer.ice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 12:47:10 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.icemortgagetechnology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:25:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ice.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: icemortgagetechnology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-knight/refs/heads/main/security/black-knight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Mortgage Technology
- Loan Servicing
- Loan Origination
- Secondary Marketing
- Default Management
- Investor Reporting
- Product Pricing Engine
- Real Estate Data
- FinTech
- Acquired Company
- ICE Mortgage Technology
---
