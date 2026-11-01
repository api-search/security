---
api_specs:
- filename: randnext-draws-api-openapi.yml
  format: yaml
  label: RandNext Draws API
  slug: randnext-draws-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/randnext/openapi/randnext-draws-api-openapi.yml
- filename: randnext-health-api-openapi.yml
  format: yaml
  label: RandNext Health API
  slug: randnext-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/randnext/openapi/randnext-health-api-openapi.yml
- filename: randnext-jokes-api-openapi.yml
  format: yaml
  label: RandNext Jokes API
  slug: randnext-jokes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/randnext/openapi/randnext-jokes-api-openapi.yml
- filename: randnext-questions-api-openapi.yml
  format: yaml
  label: RandNext Questions API
  slug: randnext-questions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/randnext/openapi/randnext-questions-api-openapi.yml
- filename: randnext-quotes-api-openapi.yml
  format: yaml
  label: RandNext Quotes API
  slug: randnext-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/randnext/openapi/randnext-quotes-api-openapi.yml
- filename: randnext-tools-api-openapi.yml
  format: yaml
  label: RandNext Tools API
  slug: randnext-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/randnext/openapi/randnext-tools-api-openapi.yml
- filename: randnext-words-api-openapi.yml
  format: yaml
  label: RandNext Words API
  slug: randnext-words-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/randnext/openapi/randnext-words-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: randnext.com
  spf: true
hosts:
- cert_expires: Jan 21 00:57:47 2027 GMT
  host: randnext.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Randnext Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RandNext, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RandNext
provider_slug: randnext
slug: randnext-domain-security
source_filename: randnext-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: randnext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 00:57:47 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: randnext.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/randnext/security/randnext-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Random
- Generator
- API
- Fun
---
