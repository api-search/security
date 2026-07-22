---
api_specs:
- filename: oper-credits-api-openapi.json
  format: json
  label: Oper Mortgage API
  slug: oper-mortgage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oper-credits/refs/heads/main/openapi/oper-credits-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: opercredits.com
  spf: true
hosts:
- cert_expires: Sep 11 16:27:43 2026 GMT
  host: opercredits.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oper Credits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oper Credits, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Oper Credits
provider_slug: oper-credits
slug: oper-credits-domain-security
source_filename: oper-credits-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opercredits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 16:27:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opercredits.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oper-credits/refs/heads/main/security/oper-credits-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Mortgages
- Lending
- Credit
- Fintech
- Banking
- Loan Origination
- Real Estate
- Financial Services
---
