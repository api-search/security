---
api_specs:
- filename: teradata-api-info-api-openapi.yml
  format: yaml
  label: Teradata API Info API
  slug: teradata-api-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-api-info-api-openapi.yml
- filename: teradata-configuration-api-openapi.yml
  format: yaml
  label: Teradata Configuration API
  slug: teradata-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-configuration-api-openapi.yml
- filename: teradata-issues-api-openapi.yml
  format: yaml
  label: Teradata Issues API
  slug: teradata-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-issues-api-openapi.yml
- filename: teradata-managers-api-openapi.yml
  format: yaml
  label: Teradata Managers API
  slug: teradata-managers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-managers-api-openapi.yml
- filename: teradata-nodes-api-openapi.yml
  format: yaml
  label: Teradata Nodes API
  slug: teradata-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-nodes-api-openapi.yml
- filename: teradata-operations-api-openapi.yml
  format: yaml
  label: Teradata Operations API
  slug: teradata-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-operations-api-openapi.yml
- filename: teradata-queries-api-openapi.yml
  format: yaml
  label: Teradata Queries API
  slug: teradata-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-queries-api-openapi.yml
- filename: teradata-sessions-api-openapi.yml
  format: yaml
  label: Teradata Sessions API
  slug: teradata-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-sessions-api-openapi.yml
- filename: teradata-software-api-openapi.yml
  format: yaml
  label: Teradata Software API
  slug: teradata-software-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-software-api-openapi.yml
- filename: teradata-systems-api-openapi.yml
  format: yaml
  label: Teradata Systems API
  slug: teradata-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-systems-api-openapi.yml
- filename: teradata-users-api-openapi.yml
  format: yaml
  label: Teradata Users API
  slug: teradata-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: teradata.com
  spf: true
hosts:
- cert_expires: Mar 31 23:59:59 2027 GMT
  host: www.teradata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: developer.teradata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: querygrid.teradata.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Teradata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teradata, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Teradata
provider_slug: teradata
slug: teradata-domain-security
source_filename: teradata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.teradata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.teradata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: querygrid.teradata.com\n  https: false\ndomains:\n- domain: teradata.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/security/teradata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Cloud
- Data Management
- Data Warehousing
- Database
- Enterprise
- Machine Learning
- SQL
- Fortune 1000
---
