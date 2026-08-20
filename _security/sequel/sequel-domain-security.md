---
api_specs:
- filename: sequel-analytics-api-openapi.yml
  format: yaml
  label: Sequel Analytics API
  slug: sequel-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-analytics-api-openapi.yml
- filename: sequel-client-api-openapi.yml
  format: yaml
  label: Sequel Client API
  slug: sequel-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-client-api-openapi.yml
- filename: sequel-company-api-openapi.yml
  format: yaml
  label: Sequel company API
  slug: sequel-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-company-api-openapi.yml
- filename: sequel-company-theme-api-openapi.yml
  format: yaml
  label: Sequel company theme API
  slug: sequel-company-theme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-company-theme-api-openapi.yml
- filename: sequel-company-theme-fonts-api-openapi.yml
  format: yaml
  label: Sequel company theme fonts API
  slug: sequel-company-theme-fonts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-company-theme-fonts-api-openapi.yml
- filename: sequel-company-theme-overrides-api-openapi.yml
  format: yaml
  label: Sequel company theme overrides API
  slug: sequel-company-theme-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-company-theme-overrides-api-openapi.yml
- filename: sequel-event-api-openapi.yml
  format: yaml
  label: Sequel event API
  slug: sequel-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-event-api-openapi.yml
- filename: sequel-event-theme-api-openapi.yml
  format: yaml
  label: Sequel event theme API
  slug: sequel-event-theme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-event-theme-api-openapi.yml
- filename: sequel-event-theme-overrides-api-openapi.yml
  format: yaml
  label: Sequel event theme overrides API
  slug: sequel-event-theme-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-event-theme-overrides-api-openapi.yml
- filename: sequel-media-api-openapi.yml
  format: yaml
  label: Sequel Media API
  slug: sequel-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-media-api-openapi.yml
- filename: sequel-networking-api-openapi.yml
  format: yaml
  label: Sequel networking API
  slug: sequel-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-networking-api-openapi.yml
- filename: sequel-platform-api-openapi.yml
  format: yaml
  label: Sequel platform API
  slug: sequel-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-platform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sequel.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: introvoke.com
  spf: true
hosts:
- cert_expires: Sep 21 14:50:13 2026 GMT
  host: sequel.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: api.introvoke.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sequel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sequel, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sequel
provider_slug: sequel
slug: sequel-domain-security
source_filename: sequel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sequel.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 14:50:13 2026 GMT\n  hsts: false\n- host: api.introvoke.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sequel.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: introvoke.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/security/sequel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Webinars
- Virtual Events
- Live Streaming
- Video
- Networking
- Marketing
- Event
- Webhook
---
