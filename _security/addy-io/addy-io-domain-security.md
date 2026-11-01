---
api_specs:
- filename: addy-io-account-details-api-openapi.yml
  format: yaml
  label: addy.io Account Details API
  slug: addy-io-account-details-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-account-details-api-openapi.yml
- filename: addy-io-account-notifications-api-openapi.yml
  format: yaml
  label: addy.io Account Notifications API
  slug: addy-io-account-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-account-notifications-api-openapi.yml
- filename: addy-io-alias-bulk-actions-api-openapi.yml
  format: yaml
  label: addy.io Alias Bulk Actions API
  slug: addy-io-alias-bulk-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-alias-bulk-actions-api-openapi.yml
- filename: addy-io-aliases-api-openapi.yml
  format: yaml
  label: addy.io Aliases API
  slug: addy-io-aliases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-aliases-api-openapi.yml
- filename: addy-io-api-token-api-openapi.yml
  format: yaml
  label: addy.io API Token API
  slug: addy-io-api-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-api-token-api-openapi.yml
- filename: addy-io-app-version-api-openapi.yml
  format: yaml
  label: addy.io App Version API
  slug: addy-io-app-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-app-version-api-openapi.yml
- filename: addy-io-blocklist-api-openapi.yml
  format: yaml
  label: addy.io Blocklist API
  slug: addy-io-blocklist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-blocklist-api-openapi.yml
- filename: addy-io-domain-options-api-openapi.yml
  format: yaml
  label: addy.io Domain Options API
  slug: addy-io-domain-options-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-domain-options-api-openapi.yml
- filename: addy-io-domains-api-openapi.yml
  format: yaml
  label: addy.io Domains API
  slug: addy-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-domains-api-openapi.yml
- filename: addy-io-endpoints-api-openapi.yml
  format: yaml
  label: addy.io Endpoints API
  slug: addy-io-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-endpoints-api-openapi.yml
- filename: addy-io-failed-deliveries-api-openapi.yml
  format: yaml
  label: addy.io Failed Deliveries API
  slug: addy-io-failed-deliveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-failed-deliveries-api-openapi.yml
- filename: addy-io-labels-api-openapi.yml
  format: yaml
  label: addy.io Labels API
  slug: addy-io-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-labels-api-openapi.yml
- filename: addy-io-recipients-api-openapi.yml
  format: yaml
  label: addy.io Recipients API
  slug: addy-io-recipients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-recipients-api-openapi.yml
- filename: addy-io-rules-api-openapi.yml
  format: yaml
  label: addy.io Rules API
  slug: addy-io-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-rules-api-openapi.yml
- filename: addy-io-usernames-api-openapi.yml
  format: yaml
  label: addy.io Usernames API
  slug: addy-io-usernames-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-usernames-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:caapolicy@addy.io"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: addy.io
  spf: true
hosts:
- host: addy.io
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Addy Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for addy.io, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: addy.io
provider_slug: addy-io
slug: addy-io-domain-security
source_filename: addy-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: addy.io\n  https: false\ndomains:\n- domain: addy.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:caapolicy@addy.io\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/addy-io/security/addy-io-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Email
- Address
- SaaS
- API
- WebApp
---
