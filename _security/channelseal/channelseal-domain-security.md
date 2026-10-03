---
api_specs:
- filename: channelseal-api-catalog-api-openapi.yml
  format: yaml
  label: ChannelSeal API Catalog API
  slug: api-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-api-catalog-api-openapi.yml
- filename: channelseal-alert-api-openapi.yml
  format: yaml
  label: ChannelSeal Alert API
  slug: channelseal-alert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-alert-api-openapi.yml
- filename: channelseal-apis-api-openapi.yml
  format: yaml
  label: ChannelSeal APIs API
  slug: channelseal-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-apis-api-openapi.yml
- filename: channelseal-application-api-openapi.yml
  format: yaml
  label: ChannelSeal Application API
  slug: channelseal-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-application-api-openapi.yml
- filename: channelseal-auditevent-api-openapi.yml
  format: yaml
  label: ChannelSeal Audit Event API
  slug: channelseal-auditevent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-auditevent-api-openapi.yml
- filename: channelseal-channel-api-openapi.yml
  format: yaml
  label: ChannelSeal Channel API
  slug: channelseal-channel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-channel-api-openapi.yml
- filename: channelseal-classification-api-openapi.yml
  format: yaml
  label: ChannelSeal Classification API
  slug: channelseal-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-classification-api-openapi.yml
- filename: channelseal-monitor-api-openapi.yml
  format: yaml
  label: ChannelSeal Monitor API
  slug: channelseal-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-monitor-api-openapi.yml
- filename: channelseal-non-human-identity-api-openapi.yml
  format: yaml
  label: ChannelSeal Non Human Identity API
  slug: channelseal-non-human-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-non-human-identity-api-openapi.yml
- filename: channelseal-sensitive-data-element-api-openapi.yml
  format: yaml
  label: ChannelSeal Sensitive Data Element API
  slug: channelseal-sensitive-data-element-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-sensitive-data-element-api-openapi.yml
- filename: channelseal-sensitive-info-group-api-openapi.yml
  format: yaml
  label: ChannelSeal Sensitive Info Group API
  slug: channelseal-sensitive-info-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-sensitive-info-group-api-openapi.yml
- filename: channelseal-sensitive-info-type-api-openapi.yml
  format: yaml
  label: ChannelSeal Sensitive Info Type API
  slug: channelseal-sensitive-info-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-sensitive-info-type-api-openapi.yml
- filename: channelseal-service-api-openapi.yml
  format: yaml
  label: ChannelSeal Service API
  slug: channelseal-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-service-api-openapi.yml
- filename: channelseal-service-provider-api-openapi.yml
  format: yaml
  label: ChannelSeal Service Provider API
  slug: channelseal-service-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-service-provider-api-openapi.yml
- filename: channelseal-summary-discovery-metrics-api-openapi.yml
  format: yaml
  label: ChannelSeal Summary Discovery Metrics API
  slug: channelseal-summary-discovery-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-summary-discovery-metrics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: channelseal.com
  spf: true
hosts:
- cert_expires: Nov  1 09:27:21 2026 GMT
  host: www.channelseal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.channelseal.com
  https: false
- host: uat.channelseal.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Channelseal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChannelSeal, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: ChannelSeal
provider_slug: channelseal
slug: channelseal-domain-security
source_filename: channelseal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.channelseal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 09:27:21 2026 GMT\n  hsts: false\n- host: api.channelseal.com\n  https: false\n- host: uat.channelseal.com\n  https: false\ndomains:\n- domain: channelseal.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/security/channelseal-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- API Security
- AI Agents
- MCP
- Data Classification
- API Discovery
- Non-Human Identity
- Sensitive Data
- Observability
- OpenTelemetry
- Governance
---
