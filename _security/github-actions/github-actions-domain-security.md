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
description: Manual probe of GitHub's hosts. The shared probe-domain-security.py excludes github.com as a domain (it is treated as a code-host for other providers), so these values were captured directly with openssl s_client, dig and an HTTP HEAD on 2026-09-17. api.githubcopilot.com is new this round — it is the host that serves GitHub's MCP server and its RFC 9728 protected-resource document, and it was not in the probe set before.
domains:
- caa:
  - digicert.com
  - globalsign.com
  - letsencrypt.org
  - sectigo.com
  caa_wildcard:
  - digicert.com
  - letsencrypt.org
  - sectigo.com
  dmarc: true
  dmarc_pct: 100
  dmarc_policy: quarantine
  dmarc_rua: mailto:dmarc@github.com
  dmarc_subdomain_policy: reject
  dnssec: false
  dnssec_note: No RRSIG records returned for github.com with +dnssec on 2026-09-17.
  domain: github.com
  spf: true
  spf_note: v=spf1 with ip4 ranges plus includes for Outlook, Google, Zendesk, Salesforce, Mailchimp (servers.mcsv.net), Marketo and SendGrid, ending ~all (softfail) rather than -all.
  spf_policy: ~all
hosts:
- cert_issuer: Sectigo Public Server Authentication CA DV E36
  cert_not_after: '2026-11-27'
  host: api.github.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_issuer: Let's Encrypt YR1
  cert_not_after: '2026-10-31'
  host: docs.github.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31557600
  hsts_preload: false
  https: true
  tls_version: TLSv1.3
- cert_issuer: Sectigo Public Server Authentication CA DV E36
  cert_not_after: '2026-11-29'
  host: github.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_issuer: Sectigo Public Server Authentication CA DV R36
  cert_not_after: '2026-10-28'
  host: api.githubcopilot.com
  hsts: false
  https: true
  note: No Strict-Transport-Security header was returned on the root; the host answers 404 at / and serves only the MCP surface.
  tls_version: TLSv1.3
hosts_probed: 4
kind: domain-security
layout: security
method: probed
name: Github Actions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GitHub Actions, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GitHub Actions
provider_slug: github-actions
slug: github-actions-domain-security
source_filename: github-actions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the GitHub API, docs, web and MCP hosts\ndescription: >-\n  Manual probe of GitHub's hosts. The shared probe-domain-security.py excludes\n  github.com as a domain (it is treated as a code-host for other providers), so\n  these values were captured directly with openssl s_client, dig and an HTTP\n  HEAD on 2026-09-17. api.githubcopilot.com is new this round — it is the host\n  that serves GitHub's MCP server and its RFC 9728 protected-resource document,\n  and it was not in the probe set before.\nhosts:\n  - {host: api.github.com, https: true, tls_version: TLSv1.3, cert_not_after: '2026-11-27', cert_issuer: Sectigo Public Server Authentication CA DV E36, hsts: true, hsts_max_age: 31536000, hsts_preload: true, hsts_include_subdomains: true}\n  - {host: docs.github.com, https: true, tls_version: TLSv1.3, cert_not_after: '2026-10-31', cert_issuer: Let's Encrypt YR1, hsts: true, hsts_max_age: 31557600,\
  \ hsts_preload: false, hsts_include_subdomains: false}\n  - {host: github.com, https: true, tls_version: TLSv1.3, cert_not_after: '2026-11-29', cert_issuer: Sectigo Public Server Authentication CA DV E36, hsts: true, hsts_max_age: 31536000, hsts_preload: true, hsts_include_subdomains: true}\n  - {host: api.githubcopilot.com, https: true, tls_version: TLSv1.3, cert_not_after: '2026-10-28', cert_issuer: Sectigo Public Server Authentication CA DV R36, hsts: false, note: 'No Strict-Transport-Security header was returned on the root; the host answers 404 at / and serves only the MCP surface.'}\ndomains:\n  - domain: github.com\n    dnssec: false\n    dnssec_note: No RRSIG records returned for github.com with +dnssec on 2026-09-17.\n    caa: ['digicert.com', 'globalsign.com', 'letsencrypt.org', 'sectigo.com']\n    caa_wildcard: ['digicert.com', 'letsencrypt.org', 'sectigo.com']\n    spf: true\n    spf_policy: ~all\n    spf_note: >-\n      v=spf1 with ip4 ranges plus includes for Outlook, Google,\
  \ Zendesk,\n      Salesforce, Mailchimp (servers.mcsv.net), Marketo and SendGrid, ending\n      ~all (softfail) rather than -all.\n    dmarc: true\n    dmarc_policy: quarantine\n    dmarc_subdomain_policy: reject\n    dmarc_pct: 100\n    dmarc_rua: mailto:dmarc@github.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/security/github-actions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CI/CD
- Continuous Integration
- Continuous Deployment
- DevOps
- Pipelines
- Workflows
- Automation
- Developer Tools
- Software Development
- Build Automation
- T1
- GitHub
---
