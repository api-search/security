---
api_specs:
- filename: numberbroom-com-credits-api-openapi.yml
  format: yaml
  label: NumberBroom Credits API
  slug: numberbroom-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/numberbroom-com/openapi/numberbroom-com-credits-api-openapi.yml
- filename: numberbroom-com-lists-api-openapi.yml
  format: yaml
  label: NumberBroom Lists API
  slug: numberbroom-com-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/numberbroom-com/openapi/numberbroom-com-lists-api-openapi.yml
- filename: numberbroom-com-verify-api-openapi.yml
  format: yaml
  label: NumberBroom Verify API
  slug: numberbroom-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/numberbroom-com/openapi/numberbroom-com-verify-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: numberbroom.com
  spf: true
hosts:
- cert_expires: Feb  9 14:05:43 2027 GMT
  host: numberbroom.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NumberBroom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NumberBroom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: NumberBroom
provider_slug: numberbroom-com
slug: numberbroom-com-domain-security
source_filename: numberbroom-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: numberbroom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 14:05:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: numberbroom.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/numberbroom-com/security/numberbroom-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Phone
- Data
- Validation
- Scrubbing
- Real Estate
---
