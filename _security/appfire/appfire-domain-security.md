---
api_specs:
- filename: appfire-api-query-methods-api-openapi.yml
  format: yaml
  label: Appfire API query methods API
  slug: appfire-api-query-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appfire/refs/heads/main/openapi/appfire-api-query-methods-api-openapi.yml
- filename: appfire-api-update-methods-api-openapi.yml
  format: yaml
  label: Appfire API update methods API
  slug: appfire-api-update-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appfire/refs/heads/main/openapi/appfire-api-update-methods-api-openapi.yml
- filename: appfire-settings-api-openapi.yml
  format: yaml
  label: Appfire Settings API
  slug: appfire-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appfire/refs/heads/main/openapi/appfire-settings-api-openapi.yml
- filename: appfire-worklogs-api-openapi.yml
  format: yaml
  label: Appfire Worklogs API
  slug: appfire-worklogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appfire/refs/heads/main/openapi/appfire-worklogs-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appfire.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: atlassian.net
  spf: true
hosts:
- cert_expires: Sep 14 11:14:05 2026 GMT
  host: appfire.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: appfire.atlassian.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 00:42:08 2026 GMT
  host: timehubjra.7pace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appfire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appfire, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Appfire
provider_slug: appfire
slug: appfire-domain-security
source_filename: appfire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appfire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 11:14:05 2026 GMT\n  hsts: null\n- host: appfire.atlassian.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: timehubjra.7pace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 00:42:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: appfire.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: atlassian.net\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild\
  \ \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appfire/refs/heads/main/security/appfire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Atlassian
- Jira
- Confluence
- Project Portfolio Management
- Work Management
- Time Tracking
- OKR
- Workflow-Automation
- Azure DevOps
- marketplace-apps
- Document Workflow
- Enterprise Software
---
