---
api_specs:
- filename: edlink-agents-api-openapi.yml
  format: yaml
  label: Edlink Agents API
  slug: edlink-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-agents-api-openapi.yml
- filename: edlink-classes-api-openapi.yml
  format: yaml
  label: Edlink Classes API
  slug: edlink-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-classes-api-openapi.yml
- filename: edlink-courses-api-openapi.yml
  format: yaml
  label: Edlink Courses API
  slug: edlink-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-courses-api-openapi.yml
- filename: edlink-districts-api-openapi.yml
  format: yaml
  label: Edlink Districts API
  slug: edlink-districts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-districts-api-openapi.yml
- filename: edlink-enrollments-api-openapi.yml
  format: yaml
  label: Edlink Enrollments API
  slug: edlink-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-enrollments-api-openapi.yml
- filename: edlink-events-api-openapi.yml
  format: yaml
  label: Edlink Events API
  slug: edlink-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-events-api-openapi.yml
- filename: edlink-graph-api-openapi.yml
  format: yaml
  label: Edlink Graph API
  slug: edlink-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-graph-api-openapi.yml
- filename: edlink-integrations-api-openapi.yml
  format: yaml
  label: Edlink Integrations API
  slug: edlink-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-integrations-api-openapi.yml
- filename: edlink-people-api-openapi.yml
  format: yaml
  label: Edlink People API
  slug: edlink-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-people-api-openapi.yml
- filename: edlink-schools-api-openapi.yml
  format: yaml
  label: Edlink Schools API
  slug: edlink-schools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-schools-api-openapi.yml
- filename: edlink-sections-api-openapi.yml
  format: yaml
  label: Edlink Sections API
  slug: edlink-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-sections-api-openapi.yml
- filename: edlink-sso-api-openapi.yml
  format: yaml
  label: Edlink SSO API
  slug: edlink-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-sso-api-openapi.yml
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
  dnssec: true
  domain: ed.link
  spf: true
hosts:
- cert_expires: Sep  5 03:39:24 2026 GMT
  host: ed.link
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Edlink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edlink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Edlink
provider_slug: edlink
slug: edlink-domain-security
source_filename: edlink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ed.link\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 03:39:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ed.link\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/security/edlink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- EdTech
- Rostering
- SIS
- LMS
- Integration
- Unified API
---
