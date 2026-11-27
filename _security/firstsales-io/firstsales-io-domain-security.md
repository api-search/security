---
api_specs:
- filename: firstsales-io-analyze-api-openapi.yml
  format: yaml
  label: FirstSales Analyze API
  slug: firstsales-io-analyze-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firstsales-io/openapi/firstsales-io-analyze-api-openapi.yml
- filename: firstsales-io-dns-api-openapi.yml
  format: yaml
  label: FirstSales DNS API
  slug: firstsales-io-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firstsales-io/openapi/firstsales-io-dns-api-openapi.yml
- filename: firstsales-io-domain-api-openapi.yml
  format: yaml
  label: FirstSales Domain API
  slug: firstsales-io-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firstsales-io/openapi/firstsales-io-domain-api-openapi.yml
- filename: firstsales-io-email-api-openapi.yml
  format: yaml
  label: FirstSales Email API
  slug: firstsales-io-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firstsales-io/openapi/firstsales-io-email-api-openapi.yml
- filename: firstsales-io-mail-tester-api-openapi.yml
  format: yaml
  label: FirstSales Mail Tester API
  slug: firstsales-io-mail-tester-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firstsales-io/openapi/firstsales-io-mail-tester-api-openapi.yml
- filename: firstsales-io-system-api-openapi.yml
  format: yaml
  label: FirstSales System API
  slug: firstsales-io-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firstsales-io/openapi/firstsales-io-system-api-openapi.yml
- filename: firstsales-io-tutorials-api-openapi.yml
  format: yaml
  label: FirstSales Tutorials API
  slug: firstsales-io-tutorials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firstsales-io/openapi/firstsales-io-tutorials-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: firstsales.io
  spf: true
hosts:
- cert_expires: Feb  3 08:21:17 2027 GMT
  host: firstsales.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FirstSales Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FirstSales, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FirstSales
provider_slug: firstsales-io
slug: firstsales-io-domain-security
source_filename: firstsales-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firstsales.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 08:21:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: firstsales.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/firstsales-io/security/firstsales-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI outbound sales
- Cold Email
- Email Warm-up
- Lead Generation
---
