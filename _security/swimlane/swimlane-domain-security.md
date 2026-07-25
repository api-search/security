---
api_specs:
- filename: swimlane-applications-api-openapi.yml
  format: yaml
  label: Swimlane Applications API
  slug: swimlane-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-applications-api-openapi.yml
- filename: swimlane-authentication-api-openapi.yml
  format: yaml
  label: Swimlane Authentication API
  slug: swimlane-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-authentication-api-openapi.yml
- filename: swimlane-groups-api-openapi.yml
  format: yaml
  label: Swimlane Groups API
  slug: swimlane-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-groups-api-openapi.yml
- filename: swimlane-logging-api-openapi.yml
  format: yaml
  label: Swimlane Logging API
  slug: swimlane-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-logging-api-openapi.yml
- filename: swimlane-records-api-openapi.yml
  format: yaml
  label: Swimlane Records API
  slug: swimlane-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-records-api-openapi.yml
- filename: swimlane-reports-api-openapi.yml
  format: yaml
  label: Swimlane Reports API
  slug: swimlane-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-reports-api-openapi.yml
- filename: swimlane-settings-api-openapi.yml
  format: yaml
  label: Swimlane Settings API
  slug: swimlane-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-settings-api-openapi.yml
- filename: swimlane-tasks-api-openapi.yml
  format: yaml
  label: Swimlane Tasks API
  slug: swimlane-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-tasks-api-openapi.yml
- filename: swimlane-users-api-openapi.yml
  format: yaml
  label: Swimlane Users API
  slug: swimlane-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/openapi/swimlane-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swimlane.com
  spf: true
hosts:
- cert_expires: Sep 10 14:59:58 2026 GMT
  host: swimlane.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 22:13:10 2026 GMT
  host: docs.swimlane.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swimlane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swimlane, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Swimlane
provider_slug: swimlane
slug: swimlane-domain-security
source_filename: swimlane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swimlane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 14:59:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.swimlane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 22:13:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: swimlane.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swimlane/refs/heads/main/security/swimlane-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SOAR
- Security Orchestration
- Automation
- Incident Response
- Playbooks
- Case Management
- Security Operations
- Agentic AI
---
