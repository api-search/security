---
api_specs:
- filename: datafold-audit-logs-api-openapi.yml
  format: yaml
  label: Datafold Audit Logs API
  slug: datafold-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-audit-logs-api-openapi.yml
- filename: datafold-bi-added-api-openapi.yml
  format: yaml
  label: Datafold bi_added API
  slug: datafold-bi-added-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-bi-added-api-openapi.yml
- filename: datafold-bi-api-openapi.yml
  format: yaml
  label: Datafold BI API
  slug: datafold-bi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-bi-api-openapi.yml
- filename: datafold-bi-deleted-api-openapi.yml
  format: yaml
  label: Datafold bi_deleted API
  slug: datafold-bi-deleted-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-bi-deleted-api-openapi.yml
- filename: datafold-bi-modified-api-openapi.yml
  format: yaml
  label: Datafold bi_modified API
  slug: datafold-bi-modified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-bi-modified-api-openapi.yml
- filename: datafold-bolt-api-openapi.yml
  format: yaml
  label: Datafold bolt API
  slug: datafold-bolt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-bolt-api-openapi.yml
- filename: datafold-ci-api-openapi.yml
  format: yaml
  label: Datafold CI API
  slug: datafold-ci-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-ci-api-openapi.yml
- filename: datafold-data-diffs-api-openapi.yml
  format: yaml
  label: Datafold Data diffs API
  slug: datafold-data-diffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-data-diffs-api-openapi.yml
- filename: datafold-data-source-added-api-openapi.yml
  format: yaml
  label: Datafold data_source_added API
  slug: datafold-data-source-added-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-data-source-added-api-openapi.yml
- filename: datafold-data-sources-api-openapi.yml
  format: yaml
  label: Datafold Data sources API
  slug: datafold-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-data-sources-api-openapi.yml
- filename: datafold-diff-created-api-openapi.yml
  format: yaml
  label: Datafold diff_created API
  slug: datafold-diff-created-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-diff-created-api-openapi.yml
- filename: datafold-explore-api-openapi.yml
  format: yaml
  label: Datafold Explore API
  slug: datafold-explore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-explore-api-openapi.yml
- filename: datafold-monitors-api-openapi.yml
  format: yaml
  label: Datafold Monitors API
  slug: datafold-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/openapi/datafold-monitors-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datafold.com
  spf: true
hosts:
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: www.datafold.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 17:31:16 2026 GMT
  host: docs.datafold.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: app.datafold.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datafold Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datafold, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Datafold
provider_slug: datafold
slug: datafold-domain-security
source_filename: datafold-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datafold.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: false\n- host: docs.datafold.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 17:31:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.datafold.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: datafold.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datafold/refs/heads/main/security/datafold-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Reliability
- Data Diff
- Data Quality
- Column-Level Lineage
- Data Pipeline
- CI/CD Integration
- Anomaly Detection
- Data Observability
- Data Migrations
---
