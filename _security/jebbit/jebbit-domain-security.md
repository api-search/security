---
api_specs:
- filename: jebbit-auth-api-openapi.yml
  format: yaml
  label: Jebbit Auth API
  slug: jebbit-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-auth-api-openapi.yml
- filename: jebbit-businesses-api-openapi.yml
  format: yaml
  label: Jebbit Businesses API
  slug: jebbit-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-businesses-api-openapi.yml
- filename: jebbit-campaigns-api-openapi.yml
  format: yaml
  label: Jebbit Campaigns API
  slug: jebbit-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-campaigns-api-openapi.yml
- filename: jebbit-feed-columns-api-openapi.yml
  format: yaml
  label: Jebbit Feed Columns API
  slug: jebbit-feed-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-feed-columns-api-openapi.yml
- filename: jebbit-feed-rows-api-openapi.yml
  format: yaml
  label: Jebbit Feed Rows API
  slug: jebbit-feed-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-feed-rows-api-openapi.yml
- filename: jebbit-feeds-api-openapi.yml
  format: yaml
  label: Jebbit Feeds API
  slug: jebbit-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-feeds-api-openapi.yml
- filename: jebbit-integration-historic-backfills-api-openapi.yml
  format: yaml
  label: Jebbit Integration Historic Backfills API
  slug: jebbit-integration-historic-backfills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-integration-historic-backfills-api-openapi.yml
- filename: jebbit-integration-mappings-api-openapi.yml
  format: yaml
  label: Jebbit Integration Mappings API
  slug: jebbit-integration-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-integration-mappings-api-openapi.yml
- filename: jebbit-integrations-api-openapi.yml
  format: yaml
  label: Jebbit Integrations API
  slug: jebbit-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-integrations-api-openapi.yml
- filename: jebbit-launch-links-api-openapi.yml
  format: yaml
  label: Jebbit Launch Links API
  slug: jebbit-launch-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-launch-links-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jebbit.com
  spf: true
hosts:
- cert_expires: Aug 24 07:32:45 2026 GMT
  host: jebbit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api2.jebbit.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jebbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jebbit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jebbit
provider_slug: jebbit
slug: jebbit-domain-security
source_filename: jebbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jebbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 07:32:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api2.jebbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: jebbit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/security/jebbit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Interactive Experiences
- Zero-Party Data
- First-Party Data
- Marketing
- Quizzes
- Product Feeds
- Webhook
- Customer Data
- JSON:API
---
