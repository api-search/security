---
api_specs:
- filename: chejefe-com-guides-api-openapi.yml
  format: yaml
  label: Jefe Guides API
  slug: chejefe-com-guides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chejefe-com/openapi/chejefe-com-guides-api-openapi.yml
- filename: chejefe-com-nlweb-api-openapi.yml
  format: yaml
  label: Jefe NL Web API
  slug: chejefe-com-nlweb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chejefe-com/openapi/chejefe-com-nlweb-api-openapi.yml
- filename: chejefe-com-product-api-openapi.yml
  format: yaml
  label: Jefe Product API
  slug: chejefe-com-product-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chejefe-com/openapi/chejefe-com-product-api-openapi.yml
- filename: chejefe-com-resources-api-openapi.yml
  format: yaml
  label: Jefe Resources API
  slug: chejefe-com-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chejefe-com/openapi/chejefe-com-resources-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chejefe.com
  spf: true
hosts:
- cert_expires: Dec  1 21:52:44 2026 GMT
  host: chejefe.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jefe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jefe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jefe
provider_slug: chejefe-com
slug: chejefe-com-domain-security
source_filename: chejefe-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chejefe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 21:52:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chejefe.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/chejefe-com/security/chejefe-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Restaurant
- WhatsApp
- Food Ordering
- Artificial Intelligence
- Online Store
- Latin America
- MCP
---
