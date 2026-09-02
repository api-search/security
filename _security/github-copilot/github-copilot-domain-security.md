---
api_specs:
- filename: github-copilot-copilot-billing-api-openapi.yml
  format: yaml
  label: GitHub Copilot Copilot Billing API
  slug: github-copilot-copilot-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/openapi/github-copilot-copilot-billing-api-openapi.yml
- filename: github-copilot-copilot-content-exclusion-api-openapi.yml
  format: yaml
  label: GitHub Copilot Copilot Content Exclusion API
  slug: github-copilot-copilot-content-exclusion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/openapi/github-copilot-copilot-content-exclusion-api-openapi.yml
- filename: github-copilot-copilot-metrics-api-openapi.yml
  format: yaml
  label: GitHub Copilot Copilot Metrics API
  slug: github-copilot-copilot-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/openapi/github-copilot-copilot-metrics-api-openapi.yml
- filename: github-copilot-copilot-seats-api-openapi.yml
  format: yaml
  label: GitHub Copilot Copilot Seats API
  slug: github-copilot-copilot-seats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/openapi/github-copilot-copilot-seats-api-openapi.yml
- filename: github-copilot-copilot-usage-reports-api-openapi.yml
  format: yaml
  label: GitHub Copilot Copilot Usage Reports API
  slug: github-copilot-copilot-usage-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/openapi/github-copilot-copilot-usage-reports-api-openapi.yml
- filename: github-copilot-copilot-user-management-api-openapi.yml
  format: yaml
  label: GitHub Copilot Copilot User Management API
  slug: github-copilot-copilot-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/openapi/github-copilot-copilot-user-management-api-openapi.yml
description: ''
domains:
- caa:
  - issue digicert.com
  - issue globalsign.com
  - issue letsencrypt.org
  - issue sectigo.com
  - issuewild digicert.com
  - issuewild letsencrypt.org
  - issuewild sectigo.com
  dmarc: true
  dmarc_policy: quarantine
  dmarc_subdomain_policy: reject
  dnssec: false
  domain: github.com
  spf: true
- caa:
  - issue digicert.com
  - issue letsencrypt.org (dns-01)
  - issue sectigo.com
  - issuewild digicert.com
  - issuewild sectigo.com
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: githubcopilot.com
  spf: true
  spf_policy: -all (hard fail)
hosts:
- cert_not_after: '2026-09-29'
  host: api.github.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_not_after: '2026-09-30'
  host: github.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_not_after: '2026-09-02'
  host: docs.github.com
  hsts: true
  hsts_max_age: 31557600
  https: true
- cert_not_after: '2026-08-30'
  host: api.githubcopilot.com
  http_status: 404
  https: true
  note: Copilot API / MCP host; root returns 404, endpoints require auth.
kind: domain-security
layout: security
method: probed
name: Github Copilot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GitHub Copilot, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GitHub Copilot
provider_slug: github-copilot
slug: github-copilot-domain-security
source_filename: github-copilot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: probed\nsource: >-\n  Live DNS/TLS/HTTP probes of the GitHub API and web hosts (2026-06-20). The\n  mechanical probe-domain-security.py excludes github.com as a code host, so\n  these hosts were probed manually with dig + openssl/curl. Absence of a record\n  (e.g. no DNSSEC) is valid recorded data.\nhosts:\n  - {host: api.github.com, https: true, tls_version: TLSv1.3, hsts: true, hsts_max_age: 31536000, hsts_preload: true, cert_not_after: '2026-09-29'}\n  - {host: github.com, https: true, tls_version: TLSv1.3, hsts: true, hsts_max_age: 31536000, hsts_preload: true, cert_not_after: '2026-09-30'}\n  - {host: docs.github.com, https: true, hsts: true, hsts_max_age: 31557600, cert_not_after: '2026-09-02'}\n  - {host: api.githubcopilot.com, https: true, http_status: 404, cert_not_after: '2026-08-30', note: 'Copilot API / MCP host; root returns 404, endpoints require auth.'}\ndomains:\n  - domain: github.com\n    dnssec: false\n    caa: ['issue digicert.com',\
  \ 'issue globalsign.com', 'issue letsencrypt.org', 'issue sectigo.com', 'issuewild digicert.com', 'issuewild letsencrypt.org', 'issuewild sectigo.com']\n    spf: true\n    dmarc: true\n    dmarc_policy: quarantine\n    dmarc_subdomain_policy: reject\n  - domain: githubcopilot.com\n    dnssec: false\n    caa: ['issue digicert.com', 'issue letsencrypt.org (dns-01)', 'issue sectigo.com', 'issuewild digicert.com', 'issuewild sectigo.com']\n    spf: true\n    spf_policy: '-all (hard fail)'\n    dmarc: true\n    dmarc_policy: reject\nnotes: >-\n  All probed hosts serve TLS 1.3 with HSTS + preload. Both registrable domains\n  publish CAA (restricting issuance to DigiCert/GlobalSign/Let's Encrypt/Sectigo),\n  SPF, and DMARC; githubcopilot.com enforces the strictest posture (SPF -all,\n  DMARC p=reject). Neither domain has DNSSEC (DS record absent).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/security/github-copilot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- Artificial Intelligence
- Code Generation
- Code Review
- Coding Agents
- Custom Instructions
- Developer Tools
- Extensions
- IDE
- Machine-Learning
- MCP
- Metrics
- Productivity
---
