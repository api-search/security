---
api_specs:
- filename: kongregate-authenticate-json-api-openapi.yml
  format: yaml
  label: Kongregate Authenticate.json API
  slug: kongregate-authenticate-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/openapi/kongregate-authenticate-json-api-openapi.yml
- filename: kongregate-characters-json-api-openapi.yml
  format: yaml
  label: Kongregate Characters.json API
  slug: kongregate-characters-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/openapi/kongregate-characters-json-api-openapi.yml
- filename: kongregate-guilds-api-openapi.yml
  format: yaml
  label: Kongregate Guilds API
  slug: kongregate-guilds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/openapi/kongregate-guilds-api-openapi.yml
- filename: kongregate-guilds-json-api-openapi.yml
  format: yaml
  label: Kongregate Guilds.json API
  slug: kongregate-guilds-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/openapi/kongregate-guilds-json-api-openapi.yml
- filename: kongregate-high-scores-api-openapi.yml
  format: yaml
  label: Kongregate High Scores API
  slug: kongregate-high-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/openapi/kongregate-high-scores-api-openapi.yml
- filename: kongregate-items-json-api-openapi.yml
  format: yaml
  label: Kongregate Items.json API
  slug: kongregate-items-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/openapi/kongregate-items-json-api-openapi.yml
- filename: kongregate-kongpanions-api-openapi.yml
  format: yaml
  label: Kongregate Kongpanions API
  slug: kongregate-kongpanions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/openapi/kongregate-kongpanions-api-openapi.yml
- filename: kongregate-kongpanions-json-api-openapi.yml
  format: yaml
  label: Kongregate Kongpanions.json API
  slug: kongregate-kongpanions-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/openapi/kongregate-kongpanions-json-api-openapi.yml
- filename: kongregate-shared-links-api-openapi.yml
  format: yaml
  label: Kongregate Shared Links API
  slug: kongregate-shared-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/openapi/kongregate-shared-links-api-openapi.yml
- filename: kongregate-submit-statistics-json-api-openapi.yml
  format: yaml
  label: Kongregate Submit Statistics.json API
  slug: kongregate-submit-statistics-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/openapi/kongregate-submit-statistics-json-api-openapi.yml
- filename: kongregate-use-item-json-api-openapi.yml
  format: yaml
  label: Kongregate Use Item.json API
  slug: kongregate-use-item-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/openapi/kongregate-use-item-json-api-openapi.yml
- filename: kongregate-user-info-json-api-openapi.yml
  format: yaml
  label: Kongregate User Info.json API
  slug: kongregate-user-info-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/openapi/kongregate-user-info-json-api-openapi.yml
- filename: kongregate-user-items-json-api-openapi.yml
  format: yaml
  label: Kongregate User Items.json API
  slug: kongregate-user-items-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/openapi/kongregate-user-items-json-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  dmarc: false
  dnssec: true
  domain: kongregate.com
  spf: true
hosts:
- cert_expires: Dec 18 15:39:08 2026 GMT
  host: www.kongregate.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 18 15:39:08 2026 GMT
  host: api.kongregate.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kongregate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kongregate, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Kongregate
provider_slug: kongregate
slug: kongregate-domain-security
source_filename: kongregate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kongregate.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 15:39:08 2026 GMT\n  hsts: false\n- host: api.kongregate.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 15:39:08 2026 GMT\n  hsts: null\ndomains:\n- domain: kongregate.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kongregate/refs/heads/main/security/kongregate-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Company
- Gaming
- Games
- Game Development
- Browser Games
- Virtual Goods
- Microtransactions
- Leaderboards
- Player Identity
- Unity
- Developer Platform
---
