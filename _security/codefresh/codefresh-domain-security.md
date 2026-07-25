---
api_specs:
- filename: codefresh-access-control-api-openapi.yml
  format: yaml
  label: Codefresh Access Control API
  slug: codefresh-access-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-access-control-api-openapi.yml
- filename: codefresh-accounts-api-openapi.yml
  format: yaml
  label: Codefresh Accounts API
  slug: codefresh-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-accounts-api-openapi.yml
- filename: codefresh-admin-api-openapi.yml
  format: yaml
  label: Codefresh Admin API
  slug: codefresh-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-admin-api-openapi.yml
- filename: codefresh-annotations-api-openapi.yml
  format: yaml
  label: Codefresh Annotations API
  slug: codefresh-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-annotations-api-openapi.yml
- filename: codefresh-audit-api-openapi.yml
  format: yaml
  label: Codefresh Audit API
  slug: codefresh-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-audit-api-openapi.yml
- filename: codefresh-auth-api-openapi.yml
  format: yaml
  label: Codefresh Auth API
  slug: codefresh-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-auth-api-openapi.yml
- filename: codefresh-builds-api-openapi.yml
  format: yaml
  label: Codefresh Builds API
  slug: codefresh-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-builds-api-openapi.yml
- filename: codefresh-clusters-api-openapi.yml
  format: yaml
  label: Codefresh Clusters API
  slug: codefresh-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-clusters-api-openapi.yml
- filename: codefresh-contexts-api-openapi.yml
  format: yaml
  label: Codefresh Contexts API
  slug: codefresh-contexts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-contexts-api-openapi.yml
- filename: codefresh-environments-api-openapi.yml
  format: yaml
  label: Codefresh Environments API
  slug: codefresh-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-environments-api-openapi.yml
- filename: codefresh-features-api-openapi.yml
  format: yaml
  label: Codefresh Features API
  slug: codefresh-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-features-api-openapi.yml
- filename: codefresh-helm-api-openapi.yml
  format: yaml
  label: Codefresh Helm API
  slug: codefresh-helm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-helm-api-openapi.yml
- filename: codefresh-workflows-api-openapi.yml
  format: yaml
  label: Codefresh Workflows API
  slug: codefresh-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/openapi/codefresh-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: codefresh.io
  spf: true
hosts:
- cert_expires: Sep 20 00:09:03 2026 GMT
  host: codefresh.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 19:29:17 2026 GMT
  host: g.codefresh.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codefresh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codefresh, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Codefresh
provider_slug: codefresh
slug: codefresh-domain-security
source_filename: codefresh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codefresh.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:09:03 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: g.codefresh.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 19:29:17 2026 GMT\n  hsts: false\ndomains:\n- domain: codefresh.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codefresh/refs/heads/main/security/codefresh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CI/CD
- Continuous Delivery
- GitOps
- Argo
- Kubernetes
- DevOps
- Pipelines
---
