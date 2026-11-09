---
api_specs:
- filename: char-gen-com-account-catalog-api-openapi.yml
  format: yaml
  label: CharGen Account & catalog API
  slug: char-gen-com-account-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-account-catalog-api-openapi.yml
- filename: char-gen-com-billing-api-openapi.yml
  format: yaml
  label: CharGen Billing API
  slug: char-gen-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-billing-api-openapi.yml
- filename: char-gen-com-entities-api-openapi.yml
  format: yaml
  label: CharGen Entities API
  slug: char-gen-com-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-entities-api-openapi.yml
- filename: char-gen-com-generations-api-openapi.yml
  format: yaml
  label: CharGen Generations API
  slug: char-gen-com-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-generations-api-openapi.yml
- filename: char-gen-com-ping-api-openapi.yml
  format: yaml
  label: CharGen Ping API
  slug: char-gen-com-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-ping-api-openapi.yml
- filename: char-gen-com-public-pricing-api-openapi.yml
  format: yaml
  label: CharGen Public pricing API
  slug: char-gen-com-public-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-public-pricing-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: char-gen.com
  spf: true
hosts:
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: char-gen.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Char Gen Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CharGen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CharGen
provider_slug: char-gen-com
slug: char-gen-com-domain-security
source_filename: char-gen-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: char-gen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: char-gen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/char-gen-com/security/char-gen-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Art
- RPG Tools
- Character Generation
- Map Generation
- Campaign Building
- Audio Generation
---
