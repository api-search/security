---
api_specs:
- filename: coorpacademy-content-openapi.json
  format: json
  label: Coorpacademy Content API
  slug: coorpacademy-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-content-openapi.json
- filename: coorpacademy-platform-openapi.json
  format: json
  label: Coorpacademy Platform API
  slug: coorpacademy-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-platform-openapi.json
- filename: coorpacademy-progression-openapi.json
  format: json
  label: Coorpacademy Progression API
  slug: coorpacademy-progression-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-progression-openapi.json
- filename: coorpacademy-progression-aggregations-openapi.json
  format: json
  label: Coorpacademy Progression Aggregations API
  slug: coorpacademy-progression-aggregations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-progression-aggregations-openapi.json
- filename: coorpacademy-scim-openapi.json
  format: json
  label: Coorpacademy SCIM API
  slug: coorpacademy-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-scim-openapi.json
- filename: coorpacademy-content-scorm-openapi.json
  format: json
  label: Coorpacademy SCORM Content API
  slug: coorpacademy-scorm-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-content-scorm-openapi.json
- filename: coorpacademy-scorm-openapi.json
  format: json
  label: Coorpacademy SCORM API
  slug: coorpacademy-scorm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-scorm-openapi.json
- filename: coorpacademy-mail-openapi.json
  format: json
  label: Coorpacademy Email API
  slug: coorpacademy-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-mail-openapi.json
- filename: coorpacademy-mobile-openapi.json
  format: json
  label: Coorpacademy Mobile API
  slug: coorpacademy-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-mobile-openapi.json
- filename: coorpacademy-review-openapi.json
  format: json
  label: Coorpacademy Review API
  slug: coorpacademy-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-review-openapi.json
- filename: coorpacademy-h5p-openapi.json
  format: json
  label: Coorpacademy H5P API
  slug: coorpacademy-h5p-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-h5p-openapi.json
- filename: coorpacademy-external-openapi.json
  format: json
  label: Coorpacademy External Resources API
  slug: coorpacademy-external-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-external-openapi.json
- filename: coorpacademy-media-openapi.json
  format: json
  label: Coorpacademy Media API
  slug: coorpacademy-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-media-openapi.json
- filename: coorpacademy-pdf-openapi.json
  format: json
  label: Coorpacademy PDF API
  slug: coorpacademy-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/openapi/coorpacademy-pdf-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coorpacademy.com
  spf: true
hosts:
- cert_expires: Oct  9 12:18:19 2026 GMT
  host: www.coorpacademy.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: api.coorpacademy.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: content.coorpacademy.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Coorpacademy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coorpacademy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Coorpacademy
provider_slug: coorpacademy
slug: coorpacademy-domain-security
source_filename: coorpacademy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coorpacademy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 12:18:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.coorpacademy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: content.coorpacademy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: coorpacademy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coorpacademy/refs/heads/main/security/coorpacademy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Saas
- corporate-learning
- lms
- learning-experience-platform
- edtech
- elearning
- scorm
- h5p
- scim
- user-provisioning
- learning-analytics
- skills
- certifications
- gamification
- france
- switzerland
---
