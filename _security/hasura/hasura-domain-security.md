---
api_specs:
- filename: hasura-asyncapi.yml
  format: yaml
  label: Hasura GraphQL API
  slug: hasura-graphql-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/asyncapi/hasura-asyncapi.yml
- filename: hasura-metadata-api-openapi.yml
  format: yaml
  label: Hasura Metadata API
  slug: hasura-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-metadata-api-openapi.yml
- filename: hasura-graphql-api-openapi.yml
  format: yaml
  label: Hasura Graphql API
  slug: hasura-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-graphql-api-openapi.yml
- filename: hasura-healthz-api-openapi.yml
  format: yaml
  label: Hasura Healthz API
  slug: hasura-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-healthz-api-openapi.yml
- filename: hasura-metadata-api-openapi.yml
  format: yaml
  label: Hasura Metadata API
  slug: hasura-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-metadata-api-openapi.yml
- filename: hasura-query-api-openapi.yml
  format: yaml
  label: Hasura Query API
  slug: hasura-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-query-api-openapi.yml
- filename: hasura-source-health-api-openapi.yml
  format: yaml
  label: Hasura Source Health API
  slug: hasura-source-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-source-health-api-openapi.yml
- filename: hasura-v1alpha1-api-openapi.yml
  format: yaml
  label: Hasura V1alpha1 API
  slug: hasura-v1alpha1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-v1alpha1-api-openapi.yml
- filename: hasura-v1beta1-api-openapi.yml
  format: yaml
  label: Hasura V1beta1 API
  slug: hasura-v1beta1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-v1beta1-api-openapi.yml
- filename: hasura-version-api-openapi.yml
  format: yaml
  label: Hasura Version API
  slug: hasura-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/openapi/hasura-version-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hasura.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: promptql.io
  spf: true
hosts:
- cert_expires: Sep 26 18:22:31 2026 GMT
  host: hasura.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 12:52:13 2026 GMT
  host: promptql.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hasura Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hasura, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hasura
provider_slug: hasura
slug: hasura-domain-security
source_filename: hasura-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hasura.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 18:22:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: promptql.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 12:52:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hasura.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: promptql.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hasura/refs/heads/main/security/hasura-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Access
- GraphQL
---
