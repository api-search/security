---
api_specs:
- filename: brightspace-assignments-api-openapi.yml
  format: yaml
  label: D2L Brightspace Assignments API
  slug: brightspace-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-assignments-api-openapi.yml
- filename: brightspace-calendar-api-openapi.yml
  format: yaml
  label: D2L Brightspace Calendar API
  slug: brightspace-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-calendar-api-openapi.yml
- filename: brightspace-content-api-openapi.yml
  format: yaml
  label: D2L Brightspace Content API
  slug: brightspace-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-content-api-openapi.yml
- filename: brightspace-data-hub-api-openapi.yml
  format: yaml
  label: D2L Brightspace Data Hub API
  slug: brightspace-data-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-data-hub-api-openapi.yml
- filename: brightspace-discussions-api-openapi.yml
  format: yaml
  label: D2L Brightspace Discussions API
  slug: brightspace-discussions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-discussions-api-openapi.yml
- filename: brightspace-enrollments-api-openapi.yml
  format: yaml
  label: D2L Brightspace Enrollments API
  slug: brightspace-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-enrollments-api-openapi.yml
- filename: brightspace-grades-api-openapi.yml
  format: yaml
  label: D2L Brightspace Grades API
  slug: brightspace-grades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-grades-api-openapi.yml
- filename: brightspace-learning-outcomes-api-openapi.yml
  format: yaml
  label: D2L Brightspace Learning Outcomes API
  slug: brightspace-learning-outcomes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-learning-outcomes-api-openapi.yml
- filename: brightspace-news-api-openapi.yml
  format: yaml
  label: D2L Brightspace News API
  slug: brightspace-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-news-api-openapi.yml
- filename: brightspace-org-units-api-openapi.yml
  format: yaml
  label: D2L Brightspace Org Units API
  slug: brightspace-org-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-org-units-api-openapi.yml
- filename: brightspace-quizzes-api-openapi.yml
  format: yaml
  label: D2L Brightspace Quizzes API
  slug: brightspace-quizzes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-quizzes-api-openapi.yml
- filename: brightspace-users-api-openapi.yml
  format: yaml
  label: D2L Brightspace Users API
  slug: brightspace-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-users-api-openapi.yml
- filename: brightspace-versions-api-openapi.yml
  format: yaml
  label: D2L Brightspace Versions API
  slug: brightspace-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/openapi/brightspace-versions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:itinfrastructureengingeering@d2l.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: d2l.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:soeplatform@d2l.com"
  - 0 issue "amazon.com"
  dmarc: false
  dnssec: true
  domain: desire2learn.com
  spf: true
hosts:
- cert_expires: Aug 17 15:35:15 2026 GMT
  host: www.d2l.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: docs.valence.desire2learn.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brightspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for D2L Brightspace, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: D2L Brightspace
provider_slug: brightspace
slug: brightspace-domain-security
source_filename: brightspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.d2l.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 15:35:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.valence.desire2learn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: d2l.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:itinfrastructureengingeering@d2l.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: desire2learn.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:soeplatform@d2l.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightspace/refs/heads/main/security/brightspace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- LMS
- Learning Management System
- EdTech
- Education
- Valence
- D2L
- Brightspace
---
