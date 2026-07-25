---
api_specs:
- filename: workleap-attributes-api-openapi.yml
  format: yaml
  label: Workleap Attributes API
  slug: workleap-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workleap/refs/heads/main/openapi/workleap-attributes-api-openapi.yml
- filename: workleap-engagement-api-openapi.yml
  format: yaml
  label: Workleap Engagement API
  slug: workleap-engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workleap/refs/heads/main/openapi/workleap-engagement-api-openapi.yml
- filename: workleap-feedback-api-openapi.yml
  format: yaml
  label: Workleap Feedback API
  slug: workleap-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workleap/refs/heads/main/openapi/workleap-feedback-api-openapi.yml
- filename: workleap-goodvibes-api-openapi.yml
  format: yaml
  label: Workleap GoodVibes API
  slug: workleap-goodvibes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workleap/refs/heads/main/openapi/workleap-goodvibes-api-openapi.yml
- filename: workleap-groups-api-openapi.yml
  format: yaml
  label: Workleap Groups API
  slug: workleap-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workleap/refs/heads/main/openapi/workleap-groups-api-openapi.yml
- filename: workleap-provisioning-api-openapi.yml
  format: yaml
  label: Workleap Provisioning API
  slug: workleap-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workleap/refs/heads/main/openapi/workleap-provisioning-api-openapi.yml
- filename: workleap-users-api-openapi.yml
  format: yaml
  label: Workleap Users API
  slug: workleap-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workleap/refs/heads/main/openapi/workleap-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: workleap.com
  spf: true
hosts:
- cert_expires: Sep  4 14:24:37 2026 GMT
  host: workleap.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 08:32:22 2026 GMT
  host: docs.api.workleap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 01:02:19 2026 GMT
  host: api.workleap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workleap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workleap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Workleap
provider_slug: workleap
slug: workleap-domain-security
source_filename: workleap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: workleap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 14:24:37 2026 GMT\n  hsts: false\n- host: docs.api.workleap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 08:32:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.workleap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 01:02:19 2026 GMT\n  hsts: null\ndomains:\n- domain: workleap.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workleap/refs/heads/main/security/workleap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Employee Experience
- HR
- Engagement
- Pulse Surveys
- Performance Management
- Officevibe
- User Provisioning
- HRIS
- Recognition
- Onboarding
---
