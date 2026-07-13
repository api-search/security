---
api_specs:
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Costs API
  slug: vantage-sh-costs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Cost Reports API
  slug: vantage-sh-cost-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Resources API
  slug: vantage-sh-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Recommendations API
  slug: vantage-sh-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Budgets API
  slug: vantage-sh-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Cost Alerts API
  slug: vantage-sh-cost-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Anomaly Alerts API
  slug: vantage-sh-anomaly-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Segments API
  slug: vantage-sh-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Financial Commitments API
  slug: vantage-sh-financial-commitments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
- filename: vantage-sh-openapi.yml
  format: yaml
  label: Vantage Dashboards API
  slug: vantage-sh-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/openapi/vantage-sh-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vantage.sh
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:_spf.salesforce.com include:46929676.spf03.hubspotemail.net ~all
hosts:
- cert_expires: Sep 29 05:23:45 2026 GMT
  host: vantage.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 11:34:18 2026 GMT
  host: www.vantage.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: api.vantage.sh
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: console.vantage.sh
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vantage Sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vantage, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vantage
provider_slug: vantage-sh
slug: vantage-sh-domain-security
source_filename: vantage-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vantage.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 05:23:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.vantage.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 11:34:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vantage.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n- host: console.vantage.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\ndomains:\n- domain: vantage.sh\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:_spf.salesforce.com include:46929676.spf03.hubspotemail.net ~all\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vantage-sh/refs/heads/main/security/vantage-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Cost
- FinOps
- Cost Management
- Cloud Optimization
- Cost Visibility
- Cloud Spend
- Multi-Cloud
---
