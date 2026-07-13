---
api_specs:
- filename: jfrog-artifactory-openapi.yml
  format: yaml
  label: JFrog Artifactory REST API
  slug: jfrog-artifactory-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-artifactory-openapi.yml
- filename: jfrog-artifactory-openapi.yml
  format: yaml
  label: JFrog Artifactory REST API V2
  slug: jfrog-artifactory-rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-artifactory-openapi.yml
- filename: jfrog-xray-openapi.yml
  format: yaml
  label: JFrog Xray REST API
  slug: jfrog-xray-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-xray-openapi.yml
- filename: jfrog-distribution-openapi.yml
  format: yaml
  label: JFrog Distribution REST API
  slug: jfrog-distribution-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-distribution-openapi.yml
- filename: jfrog-pipelines-openapi.yml
  format: yaml
  label: JFrog Pipelines REST API
  slug: jfrog-pipelines-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-pipelines-openapi.yml
- filename: jfrog-platform-openapi.yml
  format: yaml
  label: JFrog Platform REST API
  slug: jfrog-platform-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-platform-openapi.yml
- filename: jfrog-access-openapi.yml
  format: yaml
  label: JFrog Access REST API
  slug: jfrog-access-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-access-openapi.yml
- filename: jfrog-curation-openapi.yml
  format: yaml
  label: JFrog Curation REST API
  slug: jfrog-curation-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-curation-openapi.yml
- filename: jfrog-mission-control-openapi.yml
  format: yaml
  label: JFrog Mission Control REST API
  slug: jfrog-mission-control-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-mission-control-openapi.yml
- filename: jfrog-release-lifecycle-openapi.yml
  format: yaml
  label: JFrog Release Lifecycle Management REST API
  slug: jfrog-release-lifecycle-management-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-release-lifecycle-openapi.yml
- filename: jfrog-workers-openapi.yml
  format: yaml
  label: JFrog Workers REST API
  slug: jfrog-workers-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-workers-openapi.yml
- filename: jfrog-ml-openapi.yml
  format: yaml
  label: JFrog ML REST API
  slug: jfrog-ml-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-ml-openapi.yml
- filename: jfrog-connect-openapi.yml
  format: yaml
  label: JFrog Connect REST API
  slug: jfrog-connect-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-connect-openapi.yml
- filename: jfrog-catalog-openapi.yml
  format: yaml
  label: JFrog Catalog REST API
  slug: jfrog-catalog-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-catalog-openapi.yml
- filename: jfrog-evidence-openapi.yml
  format: yaml
  label: JFrog Evidence REST API
  slug: jfrog-evidence-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-evidence-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jfrog.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jfrog.io
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: jfrog.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: myserver.jfrog.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.connect.jfrog.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jfrog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JFrog, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: JFrog
provider_slug: jfrog
slug: jfrog-domain-security
source_filename: jfrog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jfrog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: myserver.jfrog.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.connect.jfrog.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: jfrog.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: jfrog.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/security/jfrog-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artifactory
- CI/CD
- Container Registry
- DevOps
- MLOps
- Package Management
- Security
- Software Supply Chain
---
