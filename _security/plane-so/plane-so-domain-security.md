---
api_specs:
- filename: plane-so-cycle-work-items-api-openapi.yml
  format: yaml
  label: Plane Cycle Work Items API
  slug: plane-so-cycle-work-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-cycle-work-items-api-openapi.yml
- filename: plane-so-cycles-api-openapi.yml
  format: yaml
  label: Plane Cycles API
  slug: plane-so-cycles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-cycles-api-openapi.yml
- filename: plane-so-labels-api-openapi.yml
  format: yaml
  label: Plane Labels API
  slug: plane-so-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-labels-api-openapi.yml
- filename: plane-so-members-api-openapi.yml
  format: yaml
  label: Plane Members API
  slug: plane-so-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-members-api-openapi.yml
- filename: plane-so-module-work-items-api-openapi.yml
  format: yaml
  label: Plane Module Work Items API
  slug: plane-so-module-work-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-module-work-items-api-openapi.yml
- filename: plane-so-modules-api-openapi.yml
  format: yaml
  label: Plane Modules API
  slug: plane-so-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-modules-api-openapi.yml
- filename: plane-so-projects-api-openapi.yml
  format: yaml
  label: Plane Projects API
  slug: plane-so-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-projects-api-openapi.yml
- filename: plane-so-states-api-openapi.yml
  format: yaml
  label: Plane States API
  slug: plane-so-states-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-states-api-openapi.yml
- filename: plane-so-work-item-comments-api-openapi.yml
  format: yaml
  label: Plane Work Item Comments API
  slug: plane-so-work-item-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-work-item-comments-api-openapi.yml
- filename: plane-so-work-item-links-api-openapi.yml
  format: yaml
  label: Plane Work Item Links API
  slug: plane-so-work-item-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-work-item-links-api-openapi.yml
- filename: plane-so-work-items-api-openapi.yml
  format: yaml
  label: Plane Work Items API
  slug: plane-so-work-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/openapi/plane-so-work-items-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:legal@plane.so"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: plane.so
  spf: true
hosts:
- cert_expires: Oct  8 05:33:03 2026 GMT
  host: plane.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 03:55:34 2026 GMT
  host: developers.plane.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 09:46:37 2026 GMT
  host: api.plane.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plane So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plane, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Plane
provider_slug: plane-so
slug: plane-so-domain-security
source_filename: plane-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plane.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:33:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.plane.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:55:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.plane.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:46:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: plane.so\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:legal@plane.so\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plane-so/refs/heads/main/security/plane-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Project Management
- Issue Tracking
- Work Management
- Open Source
- Productivity
---
