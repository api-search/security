---
api_specs:
- filename: hookdeck-connections-api-openapi.yml
  format: yaml
  label: Hookdeck Connections API
  slug: hookdeck-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-connections-api-openapi.yml
- filename: hookdeck-sources-api-openapi.yml
  format: yaml
  label: Hookdeck Sources API
  slug: hookdeck-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-sources-api-openapi.yml
- filename: hookdeck-destinations-api-openapi.yml
  format: yaml
  label: Hookdeck Destinations API
  slug: hookdeck-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-destinations-api-openapi.yml
- filename: hookdeck-events-api-openapi.yml
  format: yaml
  label: Hookdeck Events API
  slug: hookdeck-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-events-api-openapi.yml
- filename: hookdeck-requests-api-openapi.yml
  format: yaml
  label: Hookdeck Requests API
  slug: hookdeck-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-requests-api-openapi.yml
- filename: hookdeck-transformations-api-openapi.yml
  format: yaml
  label: Hookdeck Transformations API
  slug: hookdeck-transformations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-transformations-api-openapi.yml
- filename: hookdeck-bookmarks-api-openapi.yml
  format: yaml
  label: Hookdeck Bookmarks API
  slug: hookdeck-bookmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-bookmarks-api-openapi.yml
- filename: hookdeck-bulk-operations-api-openapi.yml
  format: yaml
  label: Hookdeck Bulk Operations API
  slug: hookdeck-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-bulk-operations-api-openapi.yml
- filename: hookdeck-issues-api-openapi.yml
  format: yaml
  label: Hookdeck Issues API
  slug: hookdeck-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-issues-api-openapi.yml
- filename: hookdeck-metrics-api-openapi.yml
  format: yaml
  label: Hookdeck Metrics API
  slug: hookdeck-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-metrics-api-openapi.yml
- filename: hookdeck-integrations-api-openapi.yml
  format: yaml
  label: Hookdeck Integrations API
  slug: hookdeck-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-integrations-api-openapi.yml
- filename: hookdeck-notifications-api-openapi.yml
  format: yaml
  label: Hookdeck Notifications API
  slug: hookdeck-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-notifications-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hookdeck.com
  spf: true
hosts:
- cert_expires: Sep 24 19:39:58 2026 GMT
  host: hookdeck.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 20:24:33 2026 GMT
  host: api.hookdeck.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hookdeck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hookdeck, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hookdeck
provider_slug: hookdeck
slug: hookdeck-domain-security
source_filename: hookdeck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hookdeck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 19:39:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hookdeck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 20:24:33 2026 GMT\n  hsts: null\ndomains:\n- domain: hookdeck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/security/hookdeck-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Webhooks
- Event Gateways
- Gateways
- Events
- Event Infrastructure
- Event-Driven
- Messaging
- Queues
- Retries
- Transformations
- Observability
---
