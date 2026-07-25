---
api_specs:
- filename: lattice-competencies-api-openapi.yml
  format: yaml
  label: Lattice Competencies API
  slug: lattice-competencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-competencies-api-openapi.yml
- filename: lattice-departments-api-openapi.yml
  format: yaml
  label: Lattice Departments API
  slug: lattice-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-departments-api-openapi.yml
- filename: lattice-feedbacks-api-openapi.yml
  format: yaml
  label: Lattice Feedbacks API
  slug: lattice-feedbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-feedbacks-api-openapi.yml
- filename: lattice-goal-updates-api-openapi.yml
  format: yaml
  label: Lattice Goal Updates API
  slug: lattice-goal-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-goal-updates-api-openapi.yml
- filename: lattice-goals-api-openapi.yml
  format: yaml
  label: Lattice Goals API
  slug: lattice-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-goals-api-openapi.yml
- filename: lattice-me-api-openapi.yml
  format: yaml
  label: Lattice Me API
  slug: lattice-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-me-api-openapi.yml
- filename: lattice-review-cycles-api-openapi.yml
  format: yaml
  label: Lattice Review Cycles API
  slug: lattice-review-cycles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-review-cycles-api-openapi.yml
- filename: lattice-reviewees-api-openapi.yml
  format: yaml
  label: Lattice Reviewees API
  slug: lattice-reviewees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-reviewees-api-openapi.yml
- filename: lattice-reviews-api-openapi.yml
  format: yaml
  label: Lattice Reviews API
  slug: lattice-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-reviews-api-openapi.yml
- filename: lattice-tags-api-openapi.yml
  format: yaml
  label: Lattice Tags API
  slug: lattice-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-tags-api-openapi.yml
- filename: lattice-users-api-openapi.yml
  format: yaml
  label: Lattice Users API
  slug: lattice-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lattice.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: latticehq.com
  spf: true
hosts:
- cert_expires: Sep  3 06:52:58 2026 GMT
  host: lattice.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 20:48:40 2026 GMT
  host: developers.lattice.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:00:25 2026 GMT
  host: api.latticehq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lattice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lattice, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lattice
provider_slug: lattice
slug: lattice-domain-security
source_filename: lattice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lattice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 06:52:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.lattice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:48:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.latticehq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:00:25 2026 GMT\n  hsts: false\ndomains:\n- domain: lattice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: latticehq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/security/lattice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- People Management
- Performance Management
- OKRs
- Goals
- Employee Engagement
- HRIS
- Compensation
- Feedback
- Surveys
---
