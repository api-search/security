---
api_specs:
- filename: spoken-md-balance-api-openapi.yml
  format: yaml
  label: spoken-md Balance API
  slug: spoken-md-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-balance-api-openapi.yml
- filename: spoken-md-buy-api-openapi.yml
  format: yaml
  label: spoken-md Buy API
  slug: spoken-md-buy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-buy-api-openapi.yml
- filename: spoken-md-following-api-openapi.yml
  format: yaml
  label: spoken-md Following API
  slug: spoken-md-following-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-following-api-openapi.yml
- filename: spoken-md-new-api-openapi.yml
  format: yaml
  label: spoken-md New API
  slug: spoken-md-new-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-new-api-openapi.yml
- filename: spoken-md-podcasts-api-openapi.yml
  format: yaml
  label: spoken-md Podcasts API
  slug: spoken-md-podcasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-podcasts-api-openapi.yml
- filename: spoken-md-search-api-openapi.yml
  format: yaml
  label: spoken-md Search API
  slug: spoken-md-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-search-api-openapi.yml
- filename: spoken-md-top-up-api-openapi.yml
  format: yaml
  label: spoken-md Top Up API
  slug: spoken-md-top-up-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-top-up-api-openapi.yml
- filename: spoken-md-transcripts-api-openapi.yml
  format: yaml
  label: spoken-md Transcripts API
  slug: spoken-md-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoken-md/openapi/spoken-md-transcripts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: spoken.md
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: spoken.md
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Spoken Md Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for spoken-md, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: spoken-md
provider_slug: spoken-md
slug: spoken-md-domain-security
source_filename: spoken-md-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spoken.md\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spoken.md\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/spoken-md/security/spoken-md-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- API
- Podcast
- Transcripts
- AI
- Audio
---
