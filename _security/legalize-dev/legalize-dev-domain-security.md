---
api_specs:
- filename: legalize-dev-changes-api-openapi.yml
  format: yaml
  label: Legalize Changes API
  slug: legalize-dev-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legalize-dev/openapi/legalize-dev-changes-api-openapi.yml
- filename: legalize-dev-countries-api-openapi.yml
  format: yaml
  label: Legalize Countries API
  slug: legalize-dev-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legalize-dev/openapi/legalize-dev-countries-api-openapi.yml
- filename: legalize-dev-health-api-openapi.yml
  format: yaml
  label: Legalize Health API
  slug: legalize-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legalize-dev/openapi/legalize-dev-health-api-openapi.yml
- filename: legalize-dev-jurisdictions-api-openapi.yml
  format: yaml
  label: Legalize Jurisdictions API
  slug: legalize-dev-jurisdictions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legalize-dev/openapi/legalize-dev-jurisdictions-api-openapi.yml
- filename: legalize-dev-law-types-api-openapi.yml
  format: yaml
  label: Legalize Law Types API
  slug: legalize-dev-law-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legalize-dev/openapi/legalize-dev-law-types-api-openapi.yml
- filename: legalize-dev-laws-api-openapi.yml
  format: yaml
  label: Legalize Laws API
  slug: legalize-dev-laws-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legalize-dev/openapi/legalize-dev-laws-api-openapi.yml
- filename: legalize-dev-stats-api-openapi.yml
  format: yaml
  label: Legalize Stats API
  slug: legalize-dev-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legalize-dev/openapi/legalize-dev-stats-api-openapi.yml
- filename: legalize-dev-webhooks-api-openapi.yml
  format: yaml
  label: Legalize Webhooks API
  slug: legalize-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legalize-dev/openapi/legalize-dev-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: legalize.dev
  spf: true
hosts:
- cert_expires: May 17 09:49:49 2027 GMT
  host: legalize.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Legalize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Legalize, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Legalize
provider_slug: legalize-dev
slug: legalize-dev-domain-security
source_filename: legalize-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: legalize.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 17 09:49:49 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: legalize.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/legalize-dev/security/legalize-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- OpenLegislation
- Open Source
- Data
- Transparency
- Legal Tech
---
