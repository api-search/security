---
api_specs:
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Ingest API
  slug: axiom-co-ingest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Query API (APL)
  slug: axiom-co-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Datasets API
  slug: axiom-co-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Fields API
  slug: axiom-co-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Annotations API
  slug: axiom-co-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Monitors API
  slug: axiom-co-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Notifiers API
  slug: axiom-co-notifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Dashboards API
  slug: axiom-co-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Virtual Fields API
  slug: axiom-co-virtual-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Starred Queries API
  slug: axiom-co-starred-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom API Tokens API
  slug: axiom-co-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Users API
  slug: axiom-co-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
- filename: axiom-co-openapi.yml
  format: yaml
  label: Axiom Organizations API
  slug: axiom-co-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/openapi/axiom-co-openapi.yml
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
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: api.eu.axiom.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axiom Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axiom, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Axiom
provider_slug: axiom-co
slug: axiom-co-domain-security
source_filename: axiom-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axiom.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:30:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.axiom.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\n- host: api.eu.axiom.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: axiom.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axiom-co/refs/heads/main/security/axiom-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Observability
- Log Management
- Event Data
- Logs
- Tracing
- Analytics
- APL
---
