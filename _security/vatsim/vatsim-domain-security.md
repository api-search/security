---
api_specs:
- filename: vatsim-events-api-openapi.yml
  format: yaml
  label: VATSIM Events API
  slug: vatsim-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-events-api-openapi.yml
- filename: vatsim-metar-api-openapi.yml
  format: yaml
  label: VATSIM METAR API
  slug: vatsim-metar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-metar-api-openapi.yml
- filename: vatsim-airport-info-api-openapi.yml
  format: yaml
  label: VATSIM Airport info API
  slug: vatsim-airport-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-airport-info-api-openapi.yml
- filename: vatsim-atc-api-openapi.yml
  format: yaml
  label: VATSIM atc API
  slug: vatsim-atc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-atc-api-openapi.yml
- filename: vatsim-audio-api-openapi.yml
  format: yaml
  label: VATSIM Audio API
  slug: vatsim-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-audio-api-openapi.yml
- filename: vatsim-community-api-openapi.yml
  format: yaml
  label: VATSIM community API
  slug: vatsim-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-community-api-openapi.yml
- filename: vatsim-data-feed-api-openapi.yml
  format: yaml
  label: VATSIM Data feed API
  slug: vatsim-data-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-data-feed-api-openapi.yml
- filename: vatsim-event-info-api-openapi.yml
  format: yaml
  label: VATSIM Event info API
  slug: vatsim-event-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-event-info-api-openapi.yml
- filename: vatsim-events-api-openapi.yml
  format: yaml
  label: VATSIM Events API
  slug: vatsim-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-events-api-openapi.yml
- filename: vatsim-members-api-openapi.yml
  format: yaml
  label: VATSIM members API
  slug: vatsim-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-members-api-openapi.yml
- filename: vatsim-metar-api-openapi.yml
  format: yaml
  label: VATSIM METAR API
  slug: vatsim-metar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-metar-api-openapi.yml
- filename: vatsim-oauth2-api-openapi.yml
  format: yaml
  label: VATSIM OAuth2 API
  slug: vatsim-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-oauth2-api-openapi.yml
- filename: vatsim-orgs-api-openapi.yml
  format: yaml
  label: VATSIM orgs API
  slug: vatsim-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-orgs-api-openapi.yml
- filename: vatsim-servers-api-openapi.yml
  format: yaml
  label: VATSIM Servers API
  slug: vatsim-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-servers-api-openapi.yml
- filename: vatsim-user-api-openapi.yml
  format: yaml
  label: VATSIM User API
  slug: vatsim-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-user-api-openapi.yml
- filename: vatsim-users-api-openapi.yml
  format: yaml
  label: VATSIM Users API
  slug: vatsim-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: vatsim.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: vatsim.net
  spf: true
hosts:
- cert_expires: Sep 15 13:09:37 2026 GMT
  host: vatsim.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 21:02:46 2026 GMT
  host: api.vatsim.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 21:02:46 2026 GMT
  host: data.vatsim.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vatsim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VATSIM, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: VATSIM
provider_slug: vatsim
slug: vatsim-domain-security
source_filename: vatsim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vatsim.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 13:09:37 2026 GMT\n  hsts: false\n- host: api.vatsim.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:02:46 2026 GMT\n  hsts: false\n- host: data.vatsim.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:02:46 2026 GMT\n  hsts: false\ndomains:\n- domain: vatsim.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: vatsim.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/security/vatsim-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Aviation
- Flight Simulation
- Air Traffic Control
- Real-Time Data
- Community
---
