---
api_specs:
- filename: artifactory-aql-search-api-openapi.yml
  format: yaml
  label: JFrog Artifactory AQL Search API
  slug: artifactory-aql-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-aql-search-api-openapi.yml
- filename: artifactory-artifactory-extensions-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Artifactory Extensions API
  slug: artifactory-artifactory-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-artifactory-extensions-api-openapi.yml
- filename: artifactory-artifacts-storage-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Artifacts & Storage API
  slug: artifactory-artifacts-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-artifacts-storage-api-openapi.yml
- filename: artifactory-base-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Base API
  slug: artifactory-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-base-api-openapi.yml
- filename: artifactory-blobs-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Blobs API
  slug: artifactory-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-blobs-api-openapi.yml
- filename: artifactory-build-diff-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Build Diff API
  slug: artifactory-build-diff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-build-diff-api-openapi.yml
- filename: artifactory-build-info-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Build Info API
  slug: artifactory-build-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-build-info-api-openapi.yml
- filename: artifactory-build-management-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Build Management API
  slug: artifactory-build-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-build-management-api-openapi.yml
- filename: artifactory-build-promotion-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Build Promotion API
  slug: artifactory-build-promotion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-build-promotion-api-openapi.yml
- filename: artifactory-catalog-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Catalog API
  slug: artifactory-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-catalog-api-openapi.yml
- filename: artifactory-manifests-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Manifests API
  slug: artifactory-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-manifests-api-openapi.yml
- filename: artifactory-replication-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Replication API
  slug: artifactory-replication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-replication-api-openapi.yml
- filename: artifactory-repositories-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Repositories API
  slug: artifactory-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-repositories-api-openapi.yml
- filename: artifactory-search-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Search API
  slug: artifactory-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-search-api-openapi.yml
- filename: artifactory-security-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Security API
  slug: artifactory-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-security-api-openapi.yml
- filename: artifactory-system-configuration-api-openapi.yml
  format: yaml
  label: JFrog Artifactory System & Configuration API
  slug: artifactory-system-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-system-configuration-api-openapi.yml
- filename: artifactory-tags-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Tags API
  slug: artifactory-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jfrog.com
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: jfrog.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Artifactory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JFrog Artifactory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: JFrog Artifactory
provider_slug: artifactory
slug: artifactory-domain-security
source_filename: artifactory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jfrog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jfrog.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/security/artifactory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artifacts
- DevOps
- CI/CD
- Docker Registry
- Maven
- Package Management
- Repository
---
