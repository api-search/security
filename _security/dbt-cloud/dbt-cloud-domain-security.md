---
api_specs:
- filename: dbt-cloud-openapi.yml
  format: yaml
  label: dbt Cloud Administrative API
  slug: dbt-cloud-administrative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbt-cloud/refs/heads/main/openapi/dbt-cloud-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getdbt.com
  spf: true
hosts:
- cert_expires: Sep 20 08:58:58 2026 GMT
  host: www.getdbt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 19:37:10 2026 GMT
  host: docs.getdbt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 05:21:45 2026 GMT
  host: cloud.getdbt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dbt Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dbt Cloud, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: dbt Cloud
provider_slug: dbt-cloud
slug: dbt-cloud-domain-security
source_filename: dbt-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getdbt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:58:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.getdbt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:37:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.getdbt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:21:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getdbt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dbt-cloud/refs/heads/main/security/dbt-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Analytics Engineering
- Data Transformation
- ELT
- Semantic Layer
---
