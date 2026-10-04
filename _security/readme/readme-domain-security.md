---
api_specs:
- filename: readme-personalized-docs-webhook-asyncapi.yml
  format: yaml
  label: ReadMe Personalized Docs Webhook
  slug: personalized-docs-webhook
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/asyncapi/readme-personalized-docs-webhook-asyncapi.yml
- filename: readme-analytics-api-openapi.yml
  format: yaml
  label: ReadMe Analytics API
  slug: readme-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-analytics-api-openapi.yml
- filename: readme-api-keys-api-openapi.yml
  format: yaml
  label: ReadMe API Keys API
  slug: readme-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-api-keys-api-openapi.yml
- filename: readme-branches-api-openapi.yml
  format: yaml
  label: ReadMe Branches API
  slug: readme-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-branches-api-openapi.yml
- filename: readme-categories-api-openapi.yml
  format: yaml
  label: ReadMe Categories API
  slug: readme-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-categories-api-openapi.yml
- filename: readme-changelog-api-openapi.yml
  format: yaml
  label: ReadMe Changelog API
  slug: readme-changelog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-changelog-api-openapi.yml
- filename: readme-custom-pages-api-openapi.yml
  format: yaml
  label: ReadMe Custom Pages API
  slug: readme-custom-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-custom-pages-api-openapi.yml
- filename: readme-guides-api-openapi.yml
  format: yaml
  label: ReadMe Guides API
  slug: readme-guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-guides-api-openapi.yml
- filename: readme-images-api-openapi.yml
  format: yaml
  label: ReadMe Images API
  slug: readme-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-images-api-openapi.yml
- filename: readme-metrics-api-openapi.yml
  format: yaml
  label: ReadMe Metrics API
  slug: readme-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-metrics-api-openapi.yml
- filename: readme-recipes-api-openapi.yml
  format: yaml
  label: ReadMe Recipes API
  slug: readme-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-recipes-api-openapi.yml
- filename: readme-search-api-openapi.yml
  format: yaml
  label: ReadMe Search API
  slug: readme-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-search-api-openapi.yml
- filename: readme-apis-api-openapi.yml
  format: yaml
  label: ReadMe APIs API
  slug: readme-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/openapi/readme-apis-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.com
  spf: true
hosts:
- cert_expires: Nov 11 17:09:35 2026 GMT
  host: www.readme.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 11:16:46 2026 GMT
  host: readme.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 09:30:18 2026 GMT
  host: docs.readme.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Readme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReadMe, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ReadMe
provider_slug: readme
slug: readme-domain-security
source_filename: readme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.readme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 17:09:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: readme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 11:16:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.readme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 09:30:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: readme.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/readme/refs/heads/main/security/readme-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Documentation
- Developer Hub
- API Reference
- Portal
- Analytics
- Artificial Intelligence
- MCP
- Bi-Directional Sync
- API Documentation
- Developer Portal
- OpenAPI
---
