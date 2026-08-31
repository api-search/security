---
api_specs:
- filename: channel99-ad-accounts-api-openapi.yml
  format: yaml
  label: Channel99 Ad Accounts API
  slug: channel99-ad-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-ad-accounts-api-openapi.yml
- filename: channel99-ad-campaign-groups-api-openapi.yml
  format: yaml
  label: Channel99 Ad Campaign Groups API
  slug: channel99-ad-campaign-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-ad-campaign-groups-api-openapi.yml
- filename: channel99-ad-campaigns-api-openapi.yml
  format: yaml
  label: Channel99 Ad Campaigns API
  slug: channel99-ad-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-ad-campaigns-api-openapi.yml
- filename: channel99-ad-groups-api-openapi.yml
  format: yaml
  label: Channel99 Ad Groups API
  slug: channel99-ad-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-ad-groups-api-openapi.yml
- filename: channel99-ad-units-api-openapi.yml
  format: yaml
  label: Channel99 Ad Units API
  slug: channel99-ad-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-ad-units-api-openapi.yml
- filename: channel99-ads-api-openapi.yml
  format: yaml
  label: Channel99 Ads API
  slug: channel99-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-ads-api-openapi.yml
- filename: channel99-audiences-api-openapi.yml
  format: yaml
  label: Channel99 Audiences API
  slug: channel99-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-audiences-api-openapi.yml
- filename: channel99-auth-api-openapi.yml
  format: yaml
  label: Channel99 Auth API
  slug: channel99-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-auth-api-openapi.yml
- filename: channel99-channels-api-openapi.yml
  format: yaml
  label: Channel99 Channels API
  slug: channel99-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-channels-api-openapi.yml
- filename: channel99-companies-api-openapi.yml
  format: yaml
  label: Channel99 Companies API
  slug: channel99-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-companies-api-openapi.yml
- filename: channel99-health-api-openapi.yml
  format: yaml
  label: Channel99 Health API
  slug: channel99-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-health-api-openapi.yml
- filename: channel99-impressions-api-openapi.yml
  format: yaml
  label: Channel99 Impressions API
  slug: channel99-impressions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-impressions-api-openapi.yml
- filename: channel99-intents-api-openapi.yml
  format: yaml
  label: Channel99 Intents API
  slug: channel99-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-intents-api-openapi.yml
- filename: channel99-ip-lookup-api-openapi.yml
  format: yaml
  label: Channel99 IP Lookup API
  slug: channel99-ip-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-ip-lookup-api-openapi.yml
- filename: channel99-pageviews-api-openapi.yml
  format: yaml
  label: Channel99 Pageviews API
  slug: channel99-pageviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-pageviews-api-openapi.yml
- filename: channel99-vendors-api-openapi.yml
  format: yaml
  label: Channel99 Vendors API
  slug: channel99-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-vendors-api-openapi.yml
- filename: channel99-visits-api-openapi.yml
  format: yaml
  label: Channel99 Visits API
  slug: channel99-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/openapi/channel99-visits-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: channel99.com
  spf: true
hosts:
- cert_expires: Oct  2 01:27:01 2026 GMT
  host: channel99.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:49:36 2026 GMT
  host: support.channel99.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: pulsar.channel99.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Channel99 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Channel99, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Channel99
provider_slug: channel99
slug: channel99-domain-security
source_filename: channel99-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: channel99.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 01:27:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.channel99.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:49:36 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: pulsar.channel99.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: channel99.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/security/channel99-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Analytics
- Attribution
- B2B
- Advertising
- Marketing Technology
- Artificial Intelligence
- Account Based Marketing
- Reporting
- MCP
- Agent Ready
- Intent Data
- Account Identification
- Data Export
---
