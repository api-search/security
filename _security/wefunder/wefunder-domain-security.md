---
api_specs:
- filename: wefunder-activity-api-openapi.yml
  format: yaml
  label: Wefunder Activity API
  slug: wefunder-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-activity-api-openapi.yml
- filename: wefunder-attribution-api-openapi.yml
  format: yaml
  label: Wefunder Attribution API
  slug: wefunder-attribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-attribution-api-openapi.yml
- filename: wefunder-attribution-partners-api-openapi.yml
  format: yaml
  label: Wefunder Attribution Partners API
  slug: wefunder-attribution-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-attribution-partners-api-openapi.yml
- filename: wefunder-attribution-webhooks-api-openapi.yml
  format: yaml
  label: Wefunder Attribution Webhooks API
  slug: wefunder-attribution-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-attribution-webhooks-api-openapi.yml
- filename: wefunder-campaigns-api-openapi.yml
  format: yaml
  label: Wefunder Campaigns API
  slug: wefunder-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-campaigns-api-openapi.yml
- filename: wefunder-explore-api-openapi.yml
  format: yaml
  label: Wefunder Explore API
  slug: wefunder-explore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-explore-api-openapi.yml
- filename: wefunder-intents-api-openapi.yml
  format: yaml
  label: Wefunder Intents API
  slug: wefunder-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-intents-api-openapi.yml
- filename: wefunder-investments-api-openapi.yml
  format: yaml
  label: Wefunder Investments API
  slug: wefunder-investments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-investments-api-openapi.yml
- filename: wefunder-syndicate-deals-api-openapi.yml
  format: yaml
  label: Wefunder Syndicate Deals API
  slug: wefunder-syndicate-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-syndicate-deals-api-openapi.yml
- filename: wefunder-syndicate-members-api-openapi.yml
  format: yaml
  label: Wefunder Syndicate Members API
  slug: wefunder-syndicate-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-syndicate-members-api-openapi.yml
- filename: wefunder-syndicate-statistics-api-openapi.yml
  format: yaml
  label: Wefunder Syndicate Statistics API
  slug: wefunder-syndicate-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-syndicate-statistics-api-openapi.yml
- filename: wefunder-syndicates-api-openapi.yml
  format: yaml
  label: Wefunder Syndicates API
  slug: wefunder-syndicates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-syndicates-api-openapi.yml
- filename: wefunder-users-api-openapi.yml
  format: yaml
  label: Wefunder Users API
  slug: wefunder-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wefunder.com
  spf: true
hosts:
- cert_expires: Oct  8 11:47:06 2026 GMT
  host: wefunder.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 11:47:06 2026 GMT
  host: docs.wefunder.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 11:47:06 2026 GMT
  host: api.wefunder.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wefunder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wefunder, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wefunder
provider_slug: wefunder
slug: wefunder-domain-security
source_filename: wefunder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wefunder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 11:47:06 2026 GMT\n  hsts: null\n- host: docs.wefunder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 11:47:06 2026 GMT\n  hsts: null\n- host: api.wefunder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 11:47:06 2026 GMT\n  hsts: null\ndomains:\n- domain: wefunder.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/security/wefunder-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crowdfunding
- Equity Crowdfunding
- Investing
- Fintech
- Startups
- Fundraising
- Syndicates
- Regulation Crowdfunding
---
