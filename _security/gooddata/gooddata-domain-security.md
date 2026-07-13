---
api_specs:
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Workspaces API
  slug: gooddata-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Data Sources API
  slug: gooddata-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Logical Data Model API
  slug: gooddata-logical-data-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Metrics API
  slug: gooddata-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Visualizations & Dashboards API
  slug: gooddata-visualizations-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Execution / AFM API
  slug: gooddata-execution-afm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
- filename: gooddata-openapi.yml
  format: yaml
  label: GoodData Users & Permissions API
  slug: gooddata-users-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/openapi/gooddata-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gooddata.com
  spf: true
- caa:
  - apex-loadbalancer.netlify.com.
  dmarc: false
  dnssec: true
  domain: gooddata.ai
  spf: false
hosts:
- cert_expires: Sep 26 06:33:47 2026 GMT
  host: www.gooddata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 10:03:48 2026 GMT
  host: www.gooddata.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gooddata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoodData, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GoodData
provider_slug: gooddata
slug: gooddata-domain-security
source_filename: gooddata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gooddata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 06:33:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.gooddata.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 10:03:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gooddata.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: gooddata.ai\n  dnssec: true\n  caa:\n  - apex-loadbalancer.netlify.com.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gooddata/refs/heads/main/security/gooddata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Business Intelligence
- Embedded Analytics
- Dashboards
- Data
---
