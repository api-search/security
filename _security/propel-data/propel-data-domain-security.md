---
api_specs:
- filename: propel-data-openapi.yml
  format: yaml
  label: Propel Metrics Queries API
  slug: propel-data-metrics-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propel-data/refs/heads/main/openapi/propel-data-openapi.yml
- filename: propel-data-openapi.yml
  format: yaml
  label: Propel Data Pools API
  slug: propel-data-data-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propel-data/refs/heads/main/openapi/propel-data-openapi.yml
- filename: propel-data-openapi.yml
  format: yaml
  label: Propel Data Sources API
  slug: propel-data-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propel-data/refs/heads/main/openapi/propel-data-openapi.yml
- filename: propel-data-openapi.yml
  format: yaml
  label: Propel Applications and Policies API
  slug: propel-data-applications-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propel-data/refs/heads/main/openapi/propel-data-openapi.yml
- filename: propel-data-openapi.yml
  format: yaml
  label: Propel OAuth2 Token API
  slug: propel-data-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propel-data/refs/heads/main/openapi/propel-data-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: propeldata.com
  spf: true
hosts:
- cert_expires: Dec 22 14:42:25 2026 GMT
  host: www.propeldata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.us-east-2.propeldata.com
  https: false
- host: auth.us-east-2.propeldata.com
  https: false
kind: domain-security
layout: security
method: probed
name: Propel Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Propel, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Propel
provider_slug: propel-data
slug: propel-data-domain-security
source_filename: propel-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.propeldata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 14:42:25 2026 GMT\n  hsts: false\n- host: api.us-east-2.propeldata.com\n  https: false\n- host: auth.us-east-2.propeldata.com\n  https: false\ndomains:\n- domain: propeldata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propel-data/refs/heads/main/security/propel-data-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- GraphQL
- Data Warehouse
- Metrics
- Customer Facing Analytics
---
