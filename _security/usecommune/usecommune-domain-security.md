---
api_specs:
- filename: usecommune-articles-api-openapi.yml
  format: yaml
  label: Commune Articles API
  slug: usecommune-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-articles-api-openapi.yml
- filename: usecommune-engagement-api-openapi.yml
  format: yaml
  label: Commune Engagement API
  slug: usecommune-engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-engagement-api-openapi.yml
- filename: usecommune-event-delivery-api-openapi.yml
  format: yaml
  label: Commune Event delivery API
  slug: usecommune-event-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-event-delivery-api-openapi.yml
- filename: usecommune-highlights-api-openapi.yml
  format: yaml
  label: Commune Highlights API
  slug: usecommune-highlights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-highlights-api-openapi.yml
- filename: usecommune-messages-api-openapi.yml
  format: yaml
  label: Commune Messages API
  slug: usecommune-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-messages-api-openapi.yml
- filename: usecommune-metrics-api-openapi.yml
  format: yaml
  label: Commune Metrics API
  slug: usecommune-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-metrics-api-openapi.yml
- filename: usecommune-newsletters-api-openapi.yml
  format: yaml
  label: Commune Newsletters API
  slug: usecommune-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-newsletters-api-openapi.yml
- filename: usecommune-platform-api-openapi.yml
  format: yaml
  label: Commune Platform API
  slug: usecommune-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-platform-api-openapi.yml
- filename: usecommune-search-api-openapi.yml
  format: yaml
  label: Commune Search API
  slug: usecommune-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-search-api-openapi.yml
- filename: usecommune-senders-api-openapi.yml
  format: yaml
  label: Commune Senders API
  slug: usecommune-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-senders-api-openapi.yml
- filename: usecommune-sends-api-openapi.yml
  format: yaml
  label: Commune Sends API
  slug: usecommune-sends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-sends-api-openapi.yml
- filename: usecommune-subscriber-tags-api-openapi.yml
  format: yaml
  label: Commune Subscriber tags API
  slug: usecommune-subscriber-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-subscriber-tags-api-openapi.yml
- filename: usecommune-subscribers-api-openapi.yml
  format: yaml
  label: Commune Subscribers API
  slug: usecommune-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-subscribers-api-openapi.yml
- filename: usecommune-team-api-openapi.yml
  format: yaml
  label: Commune Team API
  slug: usecommune-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-team-api-openapi.yml
- filename: usecommune-threads-api-openapi.yml
  format: yaml
  label: Commune Threads API
  slug: usecommune-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-threads-api-openapi.yml
- filename: usecommune-users-api-openapi.yml
  format: yaml
  label: Commune Users API
  slug: usecommune-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-users-api-openapi.yml
- filename: usecommune-webhooks-api-openapi.yml
  format: yaml
  label: Commune Webhooks API
  slug: usecommune-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-webhooks-api-openapi.yml
- filename: usecommune-website-domains-api-openapi.yml
  format: yaml
  label: Commune Website domains API
  slug: usecommune-website-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-website-domains-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: usecommune.com
  spf: true
hosts:
- cert_expires: Dec  1 02:55:00 2026 GMT
  host: usecommune.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Usecommune Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commune, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Commune
provider_slug: usecommune
slug: usecommune-domain-security
source_filename: usecommune-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usecommune.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 02:55:00 2026 GMT\n  hsts: false\ndomains:\n- domain: usecommune.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/security/usecommune-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Newsletters
- Email
- Community
- Publishing
- Creator Economy
- Subscribers
- Webhooks
- MCP
- Analytics
- Content
---
