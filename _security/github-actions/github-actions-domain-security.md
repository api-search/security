---
api_specs:
- filename: github-actions-artifacts-api-openapi.yml
  format: yaml
  label: GitHub Actions Artifacts API
  slug: github-actions-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-artifacts-api-openapi.yml
- filename: github-actions-cache-api-openapi.yml
  format: yaml
  label: GitHub Actions Cache API
  slug: github-actions-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-cache-api-openapi.yml
- filename: github-actions-jobs-api-openapi.yml
  format: yaml
  label: GitHub Actions Jobs API
  slug: github-actions-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-jobs-api-openapi.yml
- filename: github-actions-oidc-api-openapi.yml
  format: yaml
  label: GitHub Actions OIDC API
  slug: github-actions-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-oidc-api-openapi.yml
- filename: github-actions-permissions-api-openapi.yml
  format: yaml
  label: GitHub Actions Permissions API
  slug: github-actions-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-permissions-api-openapi.yml
- filename: github-actions-secrets-api-openapi.yml
  format: yaml
  label: GitHub Actions Secrets API
  slug: github-actions-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-secrets-api-openapi.yml
- filename: github-actions-self-hosted-runner-groups-api-openapi.yml
  format: yaml
  label: GitHub Actions Self-Hosted Runner Groups API
  slug: github-actions-self-hosted-runner-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-self-hosted-runner-groups-api-openapi.yml
- filename: github-actions-self-hosted-runners-api-openapi.yml
  format: yaml
  label: GitHub Actions Self-Hosted Runners API
  slug: github-actions-self-hosted-runners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-self-hosted-runners-api-openapi.yml
- filename: github-actions-variables-api-openapi.yml
  format: yaml
  label: GitHub Actions Variables API
  slug: github-actions-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-variables-api-openapi.yml
- filename: github-actions-workflow-runs-api-openapi.yml
  format: yaml
  label: GitHub Actions Workflow Runs API
  slug: github-actions-workflow-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-workflow-runs-api-openapi.yml
- filename: github-actions-workflows-api-openapi.yml
  format: yaml
  label: GitHub Actions Workflows API
  slug: github-actions-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-workflows-api-openapi.yml
description: Manual probe of GitHub's hosts. The shared probe-domain-security.py excludes github.com as a domain (it is treated as a code-host for other providers), so these values were captured directly with dig / openssl / HTTP HEAD.
domains:
- caa:
  - globalsign.com
  - letsencrypt.org
  - sectigo.com
  - digicert.com
  caa_wildcard:
  - digicert.com
  - letsencrypt.org
  - sectigo.com
  dmarc: true
  dmarc_policy: quarantine
  dmarc_subdomain_policy: reject
  dnssec: false
  domain: github.com
  spf: true
hosts:
- cert_not_after: '2026-09-29'
  host: api.github.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_not_after: '2026-09-02'
  host: docs.github.com
  hsts: true
  hsts_max_age: 31557600
  hsts_preload: false
  https: true
  tls_version: TLSv1.3
- cert_not_after: '2026-09-30'
  host: github.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Github Actions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GitHub Actions, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GitHub Actions
provider_slug: github-actions
slug: github-actions-domain-security
source_filename: github-actions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the GitHub API, docs and web hosts\ndescription: >-\n  Manual probe of GitHub's hosts. The shared probe-domain-security.py excludes\n  github.com as a domain (it is treated as a code-host for other providers), so\n  these values were captured directly with dig / openssl / HTTP HEAD.\nhosts:\n  - {host: api.github.com, https: true, tls_version: TLSv1.3, cert_not_after: '2026-09-29', hsts: true, hsts_max_age: 31536000, hsts_preload: true, hsts_include_subdomains: true}\n  - {host: docs.github.com, https: true, tls_version: TLSv1.3, cert_not_after: '2026-09-02', hsts: true, hsts_max_age: 31557600, hsts_preload: false}\n  - {host: github.com, https: true, tls_version: TLSv1.3, cert_not_after: '2026-09-30', hsts: true, hsts_max_age: 31536000, hsts_preload: true, hsts_include_subdomains: true}\ndomains:\n  - domain: github.com\n    dnssec: false\n    caa: ['globalsign.com', 'letsencrypt.org', 'sectigo.com',\
  \ 'digicert.com']\n    caa_wildcard: ['digicert.com', 'letsencrypt.org', 'sectigo.com']\n    spf: true\n    dmarc: true\n    dmarc_policy: quarantine\n    dmarc_subdomain_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/security/github-actions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
