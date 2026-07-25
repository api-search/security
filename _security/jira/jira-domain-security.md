---
api_specs:
- filename: jira-issue-comments-api-openapi.yml
  format: yaml
  label: Jira Issue Comments API
  slug: jira-issue-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/openapi/jira-issue-comments-api-openapi.yml
- filename: jira-issue-priorities-api-openapi.yml
  format: yaml
  label: Jira Issue Priorities API
  slug: jira-issue-priorities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/openapi/jira-issue-priorities-api-openapi.yml
- filename: jira-issue-search-api-openapi.yml
  format: yaml
  label: Jira Issue Search API
  slug: jira-issue-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/openapi/jira-issue-search-api-openapi.yml
- filename: jira-issue-statuses-api-openapi.yml
  format: yaml
  label: Jira Issue Statuses API
  slug: jira-issue-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/openapi/jira-issue-statuses-api-openapi.yml
- filename: jira-issue-transitions-api-openapi.yml
  format: yaml
  label: Jira Issue Transitions API
  slug: jira-issue-transitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/openapi/jira-issue-transitions-api-openapi.yml
- filename: jira-issue-types-api-openapi.yml
  format: yaml
  label: Jira Issue Types API
  slug: jira-issue-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/openapi/jira-issue-types-api-openapi.yml
- filename: jira-issues-api-openapi.yml
  format: yaml
  label: Jira Issues API
  slug: jira-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/openapi/jira-issues-api-openapi.yml
- filename: jira-projects-api-openapi.yml
  format: yaml
  label: Jira Projects API
  slug: jira-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/openapi/jira-projects-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: atlassian.com
  spf: true
- caa:
  - 0 issuewild "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: atlassian.net
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: developer.atlassian.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: your-domain.atlassian.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:48:31 2026 GMT
  host: help.jiraalign.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jira Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jira, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Jira
provider_slug: jira
slug: jira-domain-security
source_filename: jira-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.atlassian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: your-domain.atlassian.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.jiraalign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:48:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atlassian.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: atlassian.net\n  dnssec: false\n  caa:\n  -\
  \ 0 issuewild \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/security/jira-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
---
