---
api_specs:
- filename: microsoft-suite-calendar-api-openapi.yml
  format: yaml
  label: Microsoft Suite Calendar API
  slug: microsoft-suite-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/openapi/microsoft-suite-calendar-api-openapi.yml
- filename: microsoft-suite-files-api-openapi.yml
  format: yaml
  label: Microsoft Suite Files API
  slug: microsoft-suite-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/openapi/microsoft-suite-files-api-openapi.yml
- filename: microsoft-suite-groups-api-openapi.yml
  format: yaml
  label: Microsoft Suite Groups API
  slug: microsoft-suite-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/openapi/microsoft-suite-groups-api-openapi.yml
- filename: microsoft-suite-mail-api-openapi.yml
  format: yaml
  label: Microsoft Suite Mail API
  slug: microsoft-suite-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/openapi/microsoft-suite-mail-api-openapi.yml
- filename: microsoft-suite-subscriptions-api-openapi.yml
  format: yaml
  label: Microsoft Suite Subscriptions API
  slug: microsoft-suite-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/openapi/microsoft-suite-subscriptions-api-openapi.yml
- filename: microsoft-suite-teams-api-openapi.yml
  format: yaml
  label: Microsoft Suite Teams API
  slug: microsoft-suite-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/openapi/microsoft-suite-teams-api-openapi.yml
- filename: microsoft-suite-users-api-openapi.yml
  format: yaml
  label: Microsoft Suite Users API
  slug: microsoft-suite-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/openapi/microsoft-suite-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: graph.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Suite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Suite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Suite
provider_slug: microsoft-suite
slug: microsoft-suite-domain-security
source_filename: microsoft-suite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: graph.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-suite/refs/heads/main/security/microsoft-suite-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud
- Enterprise
- Productivity
- SaaS
---
