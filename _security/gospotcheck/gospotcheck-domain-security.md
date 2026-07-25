---
api_specs:
- filename: gospotcheck-asyncjobs-api-openapi.yml
  format: yaml
  label: GoSpotCheck AsyncJobs API
  slug: gospotcheck-asyncjobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-asyncjobs-api-openapi.yml
- filename: gospotcheck-catalogitems-api-openapi.yml
  format: yaml
  label: GoSpotCheck CatalogItems API
  slug: gospotcheck-catalogitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-catalogitems-api-openapi.yml
- filename: gospotcheck-catalogs-api-openapi.yml
  format: yaml
  label: GoSpotCheck Catalogs API
  slug: gospotcheck-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-catalogs-api-openapi.yml
- filename: gospotcheck-customviews-api-openapi.yml
  format: yaml
  label: GoSpotCheck CustomViews API
  slug: gospotcheck-customviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-customviews-api-openapi.yml
- filename: gospotcheck-missionresponses-api-openapi.yml
  format: yaml
  label: GoSpotCheck MissionResponses API
  slug: gospotcheck-missionresponses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-missionresponses-api-openapi.yml
- filename: gospotcheck-missions-api-openapi.yml
  format: yaml
  label: GoSpotCheck Missions API
  slug: gospotcheck-missions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-missions-api-openapi.yml
- filename: gospotcheck-placegroups-api-openapi.yml
  format: yaml
  label: GoSpotCheck PlaceGroups API
  slug: gospotcheck-placegroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-placegroups-api-openapi.yml
- filename: gospotcheck-places-api-openapi.yml
  format: yaml
  label: GoSpotCheck Places API
  slug: gospotcheck-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-places-api-openapi.yml
- filename: gospotcheck-taskresponses-api-openapi.yml
  format: yaml
  label: GoSpotCheck TaskResponses API
  slug: gospotcheck-taskresponses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-taskresponses-api-openapi.yml
- filename: gospotcheck-tasks-api-openapi.yml
  format: yaml
  label: GoSpotCheck Tasks API
  slug: gospotcheck-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-tasks-api-openapi.yml
- filename: gospotcheck-teams-api-openapi.yml
  format: yaml
  label: GoSpotCheck Teams API
  slug: gospotcheck-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-teams-api-openapi.yml
- filename: gospotcheck-userplaceassignments-api-openapi.yml
  format: yaml
  label: GoSpotCheck UserPlaceAssignments API
  slug: gospotcheck-userplaceassignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-userplaceassignments-api-openapi.yml
- filename: gospotcheck-users-api-openapi.yml
  format: yaml
  label: GoSpotCheck Users API
  slug: gospotcheck-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gospotcheck.com
  spf: true
hosts:
- cert_expires: Aug 31 10:16:08 2026 GMT
  host: gospotcheck.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gospotcheck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoSpotCheck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GoSpotCheck
provider_slug: gospotcheck
slug: gospotcheck-domain-security
source_filename: gospotcheck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gospotcheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 10:16:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gospotcheck.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/security/gospotcheck-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail Execution
- Field Service
- Data Collection
- Surveys
- Merchandising
- CPG
- Mobile
---
