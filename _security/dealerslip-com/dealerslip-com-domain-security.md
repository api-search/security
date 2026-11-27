---
api_specs:
- filename: dealerslip-com-invoices-api-openapi.yml
  format: yaml
  label: DealerSlip Invoices API
  slug: dealerslip-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealerslip-com/openapi/dealerslip-com-invoices-api-openapi.yml
- filename: dealerslip-com-schema-api-openapi.yml
  format: yaml
  label: DealerSlip Schema API
  slug: dealerslip-com-schema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealerslip-com/openapi/dealerslip-com-schema-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dealerslip.com
  spf: false
hosts:
- cert_expires: Feb  1 19:03:27 2027 GMT
  host: dealerslip.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DealerSlip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DealerSlip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DealerSlip
provider_slug: dealerslip-com
slug: dealerslip-com-domain-security
source_filename: dealerslip-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dealerslip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 19:03:27 2027 GMT\n  hsts: false\ndomains:\n- domain: dealerslip.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dealerslip-com/security/dealerslip-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Invoicing
- Car Sales
- UK Dealers
---
