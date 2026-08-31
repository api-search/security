---
api_specs:
- filename: firehydrant-api-openapi.yml
  format: yaml
  label: FireHydrant
  slug: firehydrant
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-api-openapi.yml
- filename: firehydrant-audits-api-openapi.yml
  format: yaml
  label: FireHydrant Audits API
  slug: firehydrant-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-audits-api-openapi.yml
- filename: firehydrant-change-events-api-openapi.yml
  format: yaml
  label: FireHydrant Change Events API
  slug: firehydrant-change-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-change-events-api-openapi.yml
- filename: firehydrant-changes-api-openapi.yml
  format: yaml
  label: FireHydrant Changes API
  slug: firehydrant-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-changes-api-openapi.yml
- filename: firehydrant-conversations-api-openapi.yml
  format: yaml
  label: FireHydrant Conversations API
  slug: firehydrant-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-conversations-api-openapi.yml
- filename: firehydrant-environments-api-openapi.yml
  format: yaml
  label: FireHydrant Environments API
  slug: firehydrant-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-environments-api-openapi.yml
- filename: firehydrant-functionalities-api-openapi.yml
  format: yaml
  label: FireHydrant Functionalities API
  slug: firehydrant-functionalities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-functionalities-api-openapi.yml
- filename: firehydrant-incidents-api-openapi.yml
  format: yaml
  label: FireHydrant Incidents API
  slug: firehydrant-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-incidents-api-openapi.yml
- filename: firehydrant-ping-api-openapi.yml
  format: yaml
  label: FireHydrant Ping API
  slug: firehydrant-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-ping-api-openapi.yml
- filename: firehydrant-priorities-api-openapi.yml
  format: yaml
  label: FireHydrant Priorities API
  slug: firehydrant-priorities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-priorities-api-openapi.yml
- filename: firehydrant-runbooks-api-openapi.yml
  format: yaml
  label: FireHydrant Runbooks API
  slug: firehydrant-runbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-runbooks-api-openapi.yml
- filename: firehydrant-scheduled-maintenances-api-openapi.yml
  format: yaml
  label: FireHydrant Scheduled Maintenances API
  slug: firehydrant-scheduled-maintenances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-scheduled-maintenances-api-openapi.yml
- filename: firehydrant-services-api-openapi.yml
  format: yaml
  label: FireHydrant Services API
  slug: firehydrant-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-services-api-openapi.yml
- filename: firehydrant-severities-api-openapi.yml
  format: yaml
  label: FireHydrant Severities API
  slug: firehydrant-severities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-severities-api-openapi.yml
- filename: firehydrant-signals-api-openapi.yml
  format: yaml
  label: FireHydrant Signals API
  slug: firehydrant-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-signals-api-openapi.yml
- filename: firehydrant-teams-api-openapi.yml
  format: yaml
  label: FireHydrant Teams API
  slug: firehydrant-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-teams-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "Digicert.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issuewild "globalsign.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: firehydrant.com
  spf: true
- caa:
  - 0 issue "Digicert.com"
  - 0 issuewild "Digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "globalsign.com"
  - 0 iodef "mailto:ops@firehydrant.io"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: firehydrant.io
  spf: true
hosts:
- cert_expires: Nov  1 21:33:51 2026 GMT
  host: firehydrant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 07:22:48 2026 GMT
  host: api.firehydrant.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Firehydrant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FireHydrant, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FireHydrant
provider_slug: firehydrant
slug: firehydrant-domain-security
source_filename: firehydrant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firehydrant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 21:33:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.firehydrant.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 07:22:48 2026 GMT\n  hsts: null\ndomains:\n- domain: firehydrant.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"Digicert.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: firehydrant.io\n  dnssec: false\n  caa:\n  - 0 issue \"Digicert.com\"\n  - 0 issuewild \"Digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 iodef \"mailto:ops@firehydrant.io\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/security/firehydrant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AIOps
- Incident Management
- On-Call
- Alerting
- Status Pages
- Runbooks
- Site Reliability Engineering
- Observability
- Retrospectives
- DevOps
---
