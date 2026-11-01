---
api_specs:
- filename: contactlint-com-openapi.json
  format: json
  label: ContactLint API
  slug: contactlint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contactlint-com/openapi/contactlint-com-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: contactlint.com
  spf: false
hosts:
- cert_expires: Jan 11 04:19:32 2027 GMT
  host: contactlint.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contactlint Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for contactlint-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: contactlint-com
provider_slug: contactlint-com
slug: contactlint-com-domain-security
source_filename: contactlint-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contactlint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 04:19:32 2027 GMT\n  hsts: null\ndomains:\n- domain: contactlint.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/contactlint-com/security/contactlint-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Email Validation
- Phone Validation
- API
- MCP
---
