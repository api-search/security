---
api_specs:
- filename: mytomorrows-legacy-graphql-proxy-api-openapi.yml
  format: yaml
  label: myTomorrows Legacy GraphQL Proxy API
  slug: mytomorrows-legacy-graphql-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-legacy-graphql-proxy-api-openapi.yml
- filename: mytomorrows-public-api-openapi.yml
  format: yaml
  label: myTomorrows Public API
  slug: mytomorrows-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-public-api-openapi.yml
- filename: mytomorrows-system-api-openapi.yml
  format: yaml
  label: myTomorrows System API
  slug: mytomorrows-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-system-api-openapi.yml
- filename: mytomorrows-anno-api-openapi.yml
  format: yaml
  label: myTomorrows Anno API
  slug: mytomorrows-anno-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-anno-api-openapi.yml
- filename: mytomorrows-autocomplete-api-openapi.yml
  format: yaml
  label: myTomorrows Autocomplete API
  slug: mytomorrows-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-autocomplete-api-openapi.yml
- filename: mytomorrows-docs-api-openapi.yml
  format: yaml
  label: myTomorrows Docs API
  slug: mytomorrows-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-docs-api-openapi.yml
- filename: mytomorrows-document-api-openapi.yml
  format: yaml
  label: myTomorrows Document API
  slug: mytomorrows-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-document-api-openapi.yml
- filename: mytomorrows-es-api-openapi.yml
  format: yaml
  label: myTomorrows Es API
  slug: mytomorrows-es-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-es-api-openapi.yml
- filename: mytomorrows-llm-api-openapi.yml
  format: yaml
  label: myTomorrows Llm API
  slug: mytomorrows-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-llm-api-openapi.yml
- filename: mytomorrows-mdt-api-openapi.yml
  format: yaml
  label: myTomorrows Mdt API
  slug: mytomorrows-mdt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-mdt-api-openapi.yml
- filename: mytomorrows-search-api-openapi.yml
  format: yaml
  label: myTomorrows Search API
  slug: mytomorrows-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-search-api-openapi.yml
- filename: mytomorrows-wrapper-api-openapi.yml
  format: yaml
  label: myTomorrows Wrapper API
  slug: mytomorrows-wrapper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-wrapper-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mytomorrows.com
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: mytomorrows.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mytomorrows Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for myTomorrows, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: myTomorrows
provider_slug: mytomorrows
slug: mytomorrows-domain-security
source_filename: mytomorrows-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mytomorrows.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mytomorrows.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/security/mytomorrows-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Clinical Trials
- Expanded Access
- Pharmaceuticals
- Patient Access
- Life Sciences
- Search
- Artificial Intelligence
---
