---
api_specs:
- filename: authenticate-methods-api-openapi.yml
  format: yaml
  label: Authenticate Methods API
  slug: authenticate-methods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/authenticate/openapi/authenticate-methods-api-openapi.yml
- filename: authenticate-mock-apis-api-openapi.yml
  format: yaml
  label: Authenticate Mock APIs API
  slug: authenticate-mock-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/authenticate/openapi/authenticate-mock-apis-api-openapi.yml
- filename: authenticate-webhooks-api-openapi.yml
  format: yaml
  label: Authenticate Webhooks API
  slug: authenticate-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/authenticate/openapi/authenticate-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: authenticate.com
  spf: true
hosts:
- cert_expires: May 20 15:43:36 2027 GMT
  host: authenticate.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Authenticate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Authenticate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Authenticate
provider_slug: authenticate
slug: authenticate-domain-security
source_filename: authenticate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: authenticate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 20 15:43:36 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: authenticate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/authenticate/security/authenticate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Identity Verification
- KBA
- Background Checks
---
