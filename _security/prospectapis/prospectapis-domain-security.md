---
api_specs:
- filename: prospectapis-pricing-api-openapi.yml
  format: yaml
  label: ProspectAPIs Pricing API
  slug: prospectapis-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-pricing-api-openapi.yml
- filename: prospectapis-watchlists-api-openapi.yml
  format: yaml
  label: ProspectAPIs Watchlists API
  slug: prospectapis-watchlists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-watchlists-api-openapi.yml
- filename: prospectapis-account-api-openapi.yml
  format: yaml
  label: ProspectAPIs Account API
  slug: prospectapis-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-account-api-openapi.yml
- filename: prospectapis-account-insights-api-openapi.yml
  format: yaml
  label: ProspectAPIs Account insights API
  slug: prospectapis-account-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-account-insights-api-openapi.yml
- filename: prospectapis-ads-api-openapi.yml
  format: yaml
  label: ProspectAPIs Ads API
  slug: prospectapis-ads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-ads-api-openapi.yml
- filename: prospectapis-companies-api-openapi.yml
  format: yaml
  label: ProspectAPIs Companies API
  slug: prospectapis-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-companies-api-openapi.yml
- filename: prospectapis-connected-account-api-openapi.yml
  format: yaml
  label: ProspectAPIs Connected account API
  slug: prospectapis-connected-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-connected-account-api-openapi.yml
- filename: prospectapis-email-verification-api-openapi.yml
  format: yaml
  label: ProspectAPIs Email verification API
  slug: prospectapis-email-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-email-verification-api-openapi.yml
- filename: prospectapis-events-api-openapi.yml
  format: yaml
  label: ProspectAPIs Events API
  slug: prospectapis-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-events-api-openapi.yml
- filename: prospectapis-funding-api-openapi.yml
  format: yaml
  label: ProspectAPIs Funding API
  slug: prospectapis-funding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-funding-api-openapi.yml
- filename: prospectapis-health-api-openapi.yml
  format: yaml
  label: ProspectAPIs Health API
  slug: prospectapis-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-health-api-openapi.yml
- filename: prospectapis-launches-api-openapi.yml
  format: yaml
  label: ProspectAPIs Launches API
  slug: prospectapis-launches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-launches-api-openapi.yml
- filename: prospectapis-messaging-reads-api-openapi.yml
  format: yaml
  label: ProspectAPIs Messaging reads API
  slug: prospectapis-messaging-reads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-messaging-reads-api-openapi.yml
- filename: prospectapis-meta-api-openapi.yml
  format: yaml
  label: ProspectAPIs Meta API
  slug: prospectapis-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-meta-api-openapi.yml
- filename: prospectapis-people-reads-api-openapi.yml
  format: yaml
  label: ProspectAPIs People reads API
  slug: prospectapis-people-reads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-people-reads-api-openapi.yml
- filename: prospectapis-people-writes-api-openapi.yml
  format: yaml
  label: ProspectAPIs People writes API
  slug: prospectapis-people-writes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-people-writes-api-openapi.yml
- filename: prospectapis-prospectapis-api-api-openapi.yml
  format: yaml
  label: ProspectAPIs ProspectAPIs API
  slug: prospectapis-prospectapis-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-prospectapis-api-api-openapi.yml
- filename: prospectapis-research-api-openapi.yml
  format: yaml
  label: ProspectAPIs Research API
  slug: prospectapis-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-research-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prospectapis.com
  spf: true
hosts:
- cert_expires: Dec 31 03:44:00 2026 GMT
  host: prospectapis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 22:47:07 2026 GMT
  host: api.prospectapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Prospectapis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ProspectAPIs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ProspectAPIs
provider_slug: prospectapis
slug: prospectapis-domain-security
source_filename: prospectapis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prospectapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 03:44:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.prospectapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 22:47:07 2026 GMT\n  hsts: null\ndomains:\n- domain: prospectapis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/prospectapis/security/prospectapis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Funding
- Research
- Data
- Funding Data
- Prospect Research
- Email Verification
- LinkedIn data
- Watchlist
- MCP
---
