---
api_specs:
- filename: teradata-querygrid-manager-api.yaml
  format: yaml
  label: Teradata QueryGrid Manager API
  slug: querygrid-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-querygrid-manager-api.yaml
- filename: teradata-query-service-api.yaml
  format: yaml
  label: Teradata Query Service API
  slug: query-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/openapi/teradata-query-service-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: teradata.com
  spf: true
hosts:
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: developer.teradata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: querygrid.teradata.com
  https: false
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: docs.teradata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teradata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teradata, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Teradata
provider_slug: teradata
slug: teradata-domain-security
source_filename: teradata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.teradata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: false\n- host: querygrid.teradata.com\n  https: false\n- host: docs.teradata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: teradata.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
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
