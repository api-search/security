---
api_specs:
- filename: university-of-amsterdam-accounts-api-openapi.yml
  format: yaml
  label: University of Amsterdam Accounts API
  slug: university-of-amsterdam-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-accounts-api-openapi.yml
- filename: university-of-amsterdam-assets-api-openapi.yml
  format: yaml
  label: University of Amsterdam Assets API
  slug: university-of-amsterdam-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-assets-api-openapi.yml
- filename: university-of-amsterdam-datasets-api-openapi.yml
  format: yaml
  label: University of Amsterdam Datasets API
  slug: university-of-amsterdam-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-datasets-api-openapi.yml
- filename: university-of-amsterdam-graphql-api-openapi.yml
  format: yaml
  label: University of Amsterdam GraphQL API
  slug: university-of-amsterdam-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-graphql-api-openapi.yml
- filename: university-of-amsterdam-graphs-api-openapi.yml
  format: yaml
  label: University of Amsterdam Graphs API
  slug: university-of-amsterdam-graphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-graphs-api-openapi.yml
- filename: university-of-amsterdam-hooks-api-openapi.yml
  format: yaml
  label: University of Amsterdam Hooks API
  slug: university-of-amsterdam-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-hooks-api-openapi.yml
- filename: university-of-amsterdam-info-api-openapi.yml
  format: yaml
  label: University of Amsterdam Info API
  slug: university-of-amsterdam-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-info-api-openapi.yml
- filename: university-of-amsterdam-jobs-api-openapi.yml
  format: yaml
  label: University of Amsterdam Jobs API
  slug: university-of-amsterdam-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-jobs-api-openapi.yml
- filename: university-of-amsterdam-prefixes-api-openapi.yml
  format: yaml
  label: University of Amsterdam Prefixes API
  slug: university-of-amsterdam-prefixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-prefixes-api-openapi.yml
- filename: university-of-amsterdam-queries-api-openapi.yml
  format: yaml
  label: University of Amsterdam Queries API
  slug: university-of-amsterdam-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-queries-api-openapi.yml
- filename: university-of-amsterdam-search-api-openapi.yml
  format: yaml
  label: University of Amsterdam Search API
  slug: university-of-amsterdam-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-search-api-openapi.yml
- filename: university-of-amsterdam-services-api-openapi.yml
  format: yaml
  label: University of Amsterdam Services API
  slug: university-of-amsterdam-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-services-api-openapi.yml
- filename: university-of-amsterdam-sparql-api-openapi.yml
  format: yaml
  label: University of Amsterdam SPARQL API
  slug: university-of-amsterdam-sparql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-sparql-api-openapi.yml
- filename: university-of-amsterdam-stories-api-openapi.yml
  format: yaml
  label: University of Amsterdam Stories API
  slug: university-of-amsterdam-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-stories-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild ";"
  - 0 iodef "mailto:scs-ra@uva.nl"
  - 0 issue "harica.gr"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uva.nl
  spf: true
hosts:
- cert_expires: Aug  6 23:59:59 2026 GMT
  host: www.uva.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: lod.uba.uva.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: api.lod.uba.uva.nl
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Amsterdam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Amsterdam, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: University of Amsterdam
provider_slug: university-of-amsterdam
slug: university-of-amsterdam-domain-security
source_filename: university-of-amsterdam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uva.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: lod.uba.uva.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lod.uba.uva.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: uva.nl\n  dnssec: true\n  caa:\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:scs-ra@uva.nl\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/security/university-of-amsterdam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Open Data
- Linked Data
- Library
- Netherlands
- Europe
---
