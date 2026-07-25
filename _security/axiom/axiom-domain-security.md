---
api_specs:
- filename: axiom-annotations-api-openapi.yml
  format: yaml
  label: Axiom Annotations API
  slug: axiom-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/openapi/axiom-annotations-api-openapi.yml
- filename: axiom-dashboards-api-openapi.yml
  format: yaml
  label: Axiom Dashboards API
  slug: axiom-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/openapi/axiom-dashboards-api-openapi.yml
- filename: axiom-datasets-api-openapi.yml
  format: yaml
  label: Axiom Datasets API
  slug: axiom-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/openapi/axiom-datasets-api-openapi.yml
- filename: axiom-edge-api-openapi.yml
  format: yaml
  label: Axiom Edge API
  slug: axiom-edge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/openapi/axiom-edge-api-openapi.yml
- filename: axiom-groups-api-openapi.yml
  format: yaml
  label: Axiom Groups API
  slug: axiom-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/openapi/axiom-groups-api-openapi.yml
- filename: axiom-mapfields-api-openapi.yml
  format: yaml
  label: Axiom Mapfields API
  slug: axiom-mapfields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/openapi/axiom-mapfields-api-openapi.yml
- filename: axiom-monitors-api-openapi.yml
  format: yaml
  label: Axiom Monitors API
  slug: axiom-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/openapi/axiom-monitors-api-openapi.yml
- filename: axiom-notifiers-api-openapi.yml
  format: yaml
  label: Axiom Notifiers API
  slug: axiom-notifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/openapi/axiom-notifiers-api-openapi.yml
- filename: axiom-orgs-api-openapi.yml
  format: yaml
  label: Axiom Orgs API
  slug: axiom-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/openapi/axiom-orgs-api-openapi.yml
- filename: axiom-roles-api-openapi.yml
  format: yaml
  label: Axiom Roles API
  slug: axiom-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/openapi/axiom-roles-api-openapi.yml
- filename: axiom-starred-api-openapi.yml
  format: yaml
  label: Axiom Starred API
  slug: axiom-starred-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/openapi/axiom-starred-api-openapi.yml
- filename: axiom-tokens-api-openapi.yml
  format: yaml
  label: Axiom Tokens API
  slug: axiom-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/openapi/axiom-tokens-api-openapi.yml
- filename: axiom-users-api-openapi.yml
  format: yaml
  label: Axiom Users API
  slug: axiom-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/openapi/axiom-users-api-openapi.yml
- filename: axiom-views-api-openapi.yml
  format: yaml
  label: Axiom Views API
  slug: axiom-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/openapi/axiom-views-api-openapi.yml
- filename: axiom-virtualfields-api-openapi.yml
  format: yaml
  label: Axiom Virtualfields API
  slug: axiom-virtualfields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/openapi/axiom-virtualfields-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: axiom.co
  spf: true
hosts:
- cert_expires: Sep 18 23:30:49 2026 GMT
  host: axiom.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: api.axiom.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axiom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axiom, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Axiom
provider_slug: axiom
slug: axiom-domain-security
source_filename: axiom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axiom.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:30:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.axiom.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: axiom.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axiom/refs/heads/main/security/axiom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Log Management
- Logging
- Observability
- Real-Time
- Serverless
---
