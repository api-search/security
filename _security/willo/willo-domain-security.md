---
api_specs:
- filename: willo-openapi.yml
  format: yaml
  label: Willo Interviews API
  slug: willo-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/openapi/willo-openapi.yml
- filename: willo-openapi.yml
  format: yaml
  label: Willo Participants (Candidates) API
  slug: willo-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/openapi/willo-openapi.yml
- filename: willo-openapi.yml
  format: yaml
  label: Willo Departments API
  slug: willo-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/openapi/willo-openapi.yml
- filename: willo-openapi.yml
  format: yaml
  label: Willo Webhooks API
  slug: willo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/openapi/willo-openapi.yml
- filename: willo-openapi.yml
  format: yaml
  label: Willo Message Templates API
  slug: willo-message-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/openapi/willo-openapi.yml
- filename: willo-openapi.yml
  format: yaml
  label: Willo Users API
  slug: willo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/openapi/willo-openapi.yml
- filename: willo-openapi.yml
  format: yaml
  label: Willo Interview Templates API
  slug: willo-interview-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/openapi/willo-openapi.yml
- filename: willo-openapi.yml
  format: yaml
  label: Willo Child Organisations API
  slug: willo-child-organisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/openapi/willo-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  - 0 iodef "mailto:support@corewide.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: willo.video
  spf: true
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@postman.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getpostman.com
  spf: true
hosts:
- cert_expires: Sep 12 12:27:02 2026 GMT
  host: www.willo.video
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 04:02:05 2026 GMT
  host: documenter.getpostman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 23:21:06 2026 GMT
  host: api.willotalent.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Willo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Willo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Willo
provider_slug: willo
slug: willo-domain-security
source_filename: willo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.willo.video\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 12:27:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documenter.getpostman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:02:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.willotalent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:21:06 2026 GMT\n  hsts: null\ndomains:\n- domain: willo.video\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:support@corewide.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: getpostman.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@postman.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  -\
  \ 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/security/willo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video Interviewing
- Recruitment
- HR Tech
- ATS
- Screening
- Async Video
---
