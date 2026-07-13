---
api_specs:
- filename: opensearch-security-openapi.yml
  format: yaml
  label: OpenSearch Security Plugin REST API
  slug: opensearch-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/openapi/opensearch-security-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opensearch.org
  spf: true
hosts:
- cert_expires: Sep  7 13:20:42 2026 GMT
  host: opensearch.org
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: docs.opensearch.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opensearch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenSearch, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenSearch
provider_slug: opensearch
slug: opensearch-domain-security
source_filename: opensearch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opensearch.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 13:20:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: docs.opensearch.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: opensearch.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/security/opensearch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- Analytics
- Observability
- Open Source
- Security
---
