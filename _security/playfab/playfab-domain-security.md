---
api_specs:
- filename: playfab-client-openapi.yml
  format: yaml
  label: PlayFab Client API
  slug: playfab-client-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-client-openapi.yml
- filename: playfab-server-openapi.yml
  format: yaml
  label: PlayFab Server API
  slug: playfab-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-server-openapi.yml
- filename: playfab-admin-openapi.yml
  format: yaml
  label: PlayFab Admin API
  slug: playfab-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-admin-openapi.yml
- filename: playfab-authentication-openapi.yml
  format: yaml
  label: PlayFab Authentication API
  slug: playfab-entity-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-authentication-openapi.yml
- filename: playfab-cloudscript-openapi.yml
  format: yaml
  label: PlayFab CloudScript API
  slug: playfab-cloudscript-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-cloudscript-openapi.yml
- filename: playfab-multiplayer-openapi.yml
  format: yaml
  label: PlayFab Multiplayer API
  slug: playfab-multiplayer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-multiplayer-openapi.yml
- filename: playfab-economy-openapi.yml
  format: yaml
  label: PlayFab Economy (Catalog / Inventory) API
  slug: playfab-economy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-economy-openapi.yml
- filename: playfab-data-openapi.yml
  format: yaml
  label: PlayFab Data API
  slug: playfab-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-data-openapi.yml
- filename: playfab-groups-openapi.yml
  format: yaml
  label: PlayFab Groups API
  slug: playfab-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-groups-openapi.yml
- filename: playfab-profiles-openapi.yml
  format: yaml
  label: PlayFab Profiles API
  slug: playfab-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-profiles-openapi.yml
- filename: playfab-events-openapi.yml
  format: yaml
  label: PlayFab Events API
  slug: playfab-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-events-openapi.yml
- filename: playfab-insights-openapi.yml
  format: yaml
  label: PlayFab Insights API
  slug: playfab-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-insights-openapi.yml
- filename: playfab-localization-openapi.yml
  format: yaml
  label: PlayFab Localization API
  slug: playfab-localization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-localization-openapi.yml
- filename: playfab-addon-openapi.yml
  format: yaml
  label: PlayFab Addon API
  slug: playfab-addon-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-addon-openapi.yml
- filename: playfab-experimentation-openapi.yml
  format: yaml
  label: PlayFab Experimentation API
  slug: playfab-experimentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-experimentation-openapi.yml
- filename: playfab-leaderboards-openapi.yml
  format: yaml
  label: PlayFab Leaderboards API
  slug: playfab-leaderboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-leaderboards-openapi.yml
- filename: playfab-progression-openapi.yml
  format: yaml
  label: PlayFab Progression API
  slug: playfab-progression-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-progression-openapi.yml
- filename: playfab-account-api-openapi.yml
  format: yaml
  label: PlayFab Account API
  slug: playfab-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-account-api-openapi.yml
- filename: playfab-authentication-api-openapi.yml
  format: yaml
  label: PlayFab Authentication API
  slug: playfab-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playfab/openapi/playfab-authentication-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "microsoft.com"
  - 128 contactemail "caarecordaware@microsoft.com"
  - 0 iodef "mailto:caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: playfab.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: playfab.com
  hsts: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 25 14:55:00 2027 GMT
  host: developer.playfab.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 00:23:13 2027 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Playfab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlayFab, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PlayFab
provider_slug: playfab
slug: playfab-domain-security
source_filename: playfab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: playfab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n- host: developer.playfab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 14:55:00 2027 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: playfab.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"microsoft.com\"\n  - 128 contactemail \"caarecordaware@microsoft.com\"\n  - 0 iodef \"mailto:caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/playfab/security/playfab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Microsoft Azure
- Backend
- Backend-as-a-Service
- CloudScript
- Economy
- Game Backend
- Game Development
- Games
- Leaderboards
- Matchmaking
- Microsoft
- Multiplayer
- PlayFab
- REST
---
