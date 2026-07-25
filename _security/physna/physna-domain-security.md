---
api_specs:
- filename: physna-clientcredentials-api-openapi.yml
  format: yaml
  label: Physna ClientCredentials API
  slug: physna-clientcredentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/physna/refs/heads/main/openapi/physna-clientcredentials-api-openapi.yml
- filename: physna-collections-api-openapi.yml
  format: yaml
  label: Physna Collections API
  slug: physna-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/physna/refs/heads/main/openapi/physna-collections-api-openapi.yml
- filename: physna-deprecated-api-openapi.yml
  format: yaml
  label: Physna Deprecated API
  slug: physna-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/physna/refs/heads/main/openapi/physna-deprecated-api-openapi.yml
- filename: physna-folders-api-openapi.yml
  format: yaml
  label: Physna Folders API
  slug: physna-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/physna/refs/heads/main/openapi/physna-folders-api-openapi.yml
- filename: physna-image-search-api-openapi.yml
  format: yaml
  label: Physna Image Search API
  slug: physna-image-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/physna/refs/heads/main/openapi/physna-image-search-api-openapi.yml
- filename: physna-metadata-api-openapi.yml
  format: yaml
  label: Physna Metadata API
  slug: physna-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/physna/refs/heads/main/openapi/physna-metadata-api-openapi.yml
- filename: physna-models-api-openapi.yml
  format: yaml
  label: Physna Models API
  slug: physna-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/physna/refs/heads/main/openapi/physna-models-api-openapi.yml
- filename: physna-users-api-openapi.yml
  format: yaml
  label: Physna Users API
  slug: physna-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/physna/refs/heads/main/openapi/physna-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: physna.com
  spf: true
hosts:
- cert_expires: Aug 20 23:57:29 2026 GMT
  host: www.physna.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 00:32:28 2026 GMT
  host: api.physna.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Physna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Physna, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Physna
provider_slug: physna
slug: physna-domain-security
source_filename: physna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.physna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:57:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.physna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 00:32:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: physna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/physna/refs/heads/main/security/physna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- 3D
- Geometric Search
- Manufacturing
- Engineering
- Machine Learning
- Search
- Computer Vision
- Product Development
---
