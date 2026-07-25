---
api_specs:
- filename: precog-admin-api-openapi.yml
  format: yaml
  label: Precog Admin API
  slug: precog-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-admin-api-openapi.yml
- filename: precog-data-model-api-openapi.yml
  format: yaml
  label: Precog Data Model API
  slug: precog-data-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-data-model-api-openapi.yml
- filename: precog-datasets-api-openapi.yml
  format: yaml
  label: Precog Datasets API
  slug: precog-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-datasets-api-openapi.yml
- filename: precog-destinations-api-openapi.yml
  format: yaml
  label: Precog Destinations API
  slug: precog-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-destinations-api-openapi.yml
- filename: precog-issues-api-openapi.yml
  format: yaml
  label: Precog Issues API
  slug: precog-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-issues-api-openapi.yml
- filename: precog-kinds-api-openapi.yml
  format: yaml
  label: Precog Kinds API
  slug: precog-kinds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-kinds-api-openapi.yml
- filename: precog-loads-api-openapi.yml
  format: yaml
  label: Precog Loads API
  slug: precog-loads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-loads-api-openapi.yml
- filename: precog-log-api-openapi.yml
  format: yaml
  label: Precog Log API
  slug: precog-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-log-api-openapi.yml
- filename: precog-pipelines-api-openapi.yml
  format: yaml
  label: Precog Pipelines API
  slug: precog-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-pipelines-api-openapi.yml
- filename: precog-semantic-model-api-openapi.yml
  format: yaml
  label: Precog Semantic Model API
  slug: precog-semantic-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-semantic-model-api-openapi.yml
- filename: precog-sources-api-openapi.yml
  format: yaml
  label: Precog Sources API
  slug: precog-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-sources-api-openapi.yml
- filename: precog-stripe-api-openapi.yml
  format: yaml
  label: Precog Stripe API
  slug: precog-stripe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/openapi/precog-stripe-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: precog.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: precog.cloud
  spf: false
hosts:
- cert_expires: Aug 27 06:49:11 2026 GMT
  host: precog.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 03:07:10 2026 GMT
  host: studio.precog.cloud
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 10:00:36 2026 GMT
  host: api.precog.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Precog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Precog, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Precog
provider_slug: precog
slug: precog-domain-security
source_filename: precog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: precog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 06:49:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: studio.precog.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 03:07:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.precog.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 10:00:36 2026 GMT\n  hsts: null\ndomains:\n- domain: precog.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: precog.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/precog/refs/heads/main/security/precog-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Integration
- ETL
- Artificial Intelligence
- Semantic Layer
- Model Context Protocol
- Data Pipelines
- Analytics
- Enterprise
---
