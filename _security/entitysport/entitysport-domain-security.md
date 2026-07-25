---
api_specs:
- filename: entitysport-authentication-api-openapi.yml
  format: yaml
  label: Entity Sport Authentication API
  slug: entitysport-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-authentication-api-openapi.yml
- filename: entitysport-competitions-api-openapi.yml
  format: yaml
  label: Entity Sport Competitions API
  slug: entitysport-competitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-competitions-api-openapi.yml
- filename: entitysport-fantasy-api-openapi.yml
  format: yaml
  label: Entity Sport Fantasy API
  slug: entitysport-fantasy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-fantasy-api-openapi.yml
- filename: entitysport-matches-api-openapi.yml
  format: yaml
  label: Entity Sport Matches API
  slug: entitysport-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-matches-api-openapi.yml
- filename: entitysport-odds-api-openapi.yml
  format: yaml
  label: Entity Sport Odds API
  slug: entitysport-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-odds-api-openapi.yml
- filename: entitysport-players-api-openapi.yml
  format: yaml
  label: Entity Sport Players API
  slug: entitysport-players-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-players-api-openapi.yml
- filename: entitysport-scorecards-api-openapi.yml
  format: yaml
  label: Entity Sport Scorecards API
  slug: entitysport-scorecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-scorecards-api-openapi.yml
- filename: entitysport-teams-api-openapi.yml
  format: yaml
  label: Entity Sport Teams API
  slug: entitysport-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/openapi/entitysport-teams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: entitysport.com
  spf: true
hosts:
- cert_expires: Aug 28 10:01:49 2026 GMT
  host: www.entitysport.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 04:01:42 2026 GMT
  host: www.doc.entitysport.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 05:13:21 2026 GMT
  host: restapi.entitysport.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Entitysport Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Entity Sport, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Entity Sport
provider_slug: entitysport
slug: entitysport-domain-security
source_filename: entitysport-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.entitysport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 10:01:49 2026 GMT\n  hsts: false\n- host: www.doc.entitysport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 04:01:42 2026 GMT\n  hsts: false\n- host: restapi.entitysport.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 05:13:21 2026 GMT\n  hsts: false\ndomains:\n- domain: entitysport.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entitysport/refs/heads/main/security/entitysport-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sports Data
- Cricket
- Live Scores
- Fantasy
- Odds
---
