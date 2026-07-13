---
api_specs:
- filename: edlink-openapi.yml
  format: yaml
  label: Graph API - Users, Classes, Enrollments
  slug: graph-users-classes-enrollments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-openapi.yml
- filename: edlink-openapi.yml
  format: yaml
  label: Graph API - Schools, Districts
  slug: graph-schools-districts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-openapi.yml
- filename: edlink-openapi.yml
  format: yaml
  label: Graph API - Courses, Sections
  slug: graph-courses-sections
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-openapi.yml
- filename: edlink-openapi.yml
  format: yaml
  label: SSO
  slug: sso
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-openapi.yml
- filename: edlink-openapi.yml
  format: yaml
  label: Sources, Integrations
  slug: sources-integrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-openapi.yml
- filename: edlink-openapi.yml
  format: yaml
  label: Events, Webhooks
  slug: events-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-openapi.yml
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
