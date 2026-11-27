---
api_specs:
- filename: gocodebook-com-jurisdictions-api-openapi.yml
  format: yaml
  label: GoCodebook Jurisdictions API
  slug: gocodebook-com-jurisdictions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gocodebook-com/openapi/gocodebook-com-jurisdictions-api-openapi.yml
- filename: gocodebook-com-search-api-openapi.yml
  format: yaml
  label: GoCodebook Search API
  slug: gocodebook-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gocodebook-com/openapi/gocodebook-com-search-api-openapi.yml
- filename: gocodebook-com-topics-api-openapi.yml
  format: yaml
  label: GoCodebook Topics API
  slug: gocodebook-com-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gocodebook-com/openapi/gocodebook-com-topics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gocodebook.com
  spf: true
hosts:
- cert_expires: Jan  6 04:51:35 2027 GMT
  host: gocodebook.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GoCodebook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoCodebook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GoCodebook
provider_slug: gocodebook-com
slug: gocodebook-com-domain-security
source_filename: gocodebook-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gocodebook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 04:51:35 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gocodebook.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gocodebook-com/security/gocodebook-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Building Codes
- Real Estate Law
- Zoning
- AI Research
- Construction
---
