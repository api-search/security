---
api_specs:
- filename: 360learning-authentication-api-openapi.yml
  format: yaml
  label: 360Learning Authentication API
  slug: 360learning-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-authentication-api-openapi.yml
- filename: 360learning-certificate-outlines-api-openapi.yml
  format: yaml
  label: 360Learning Certificate Outlines API
  slug: 360learning-certificate-outlines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-certificate-outlines-api-openapi.yml
- filename: 360learning-classrooms-api-openapi.yml
  format: yaml
  label: 360Learning Classrooms API
  slug: 360learning-classrooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-classrooms-api-openapi.yml
- filename: 360learning-courses-api-openapi.yml
  format: yaml
  label: 360Learning Courses API
  slug: 360learning-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-courses-api-openapi.yml
- filename: 360learning-custom-fields-api-openapi.yml
  format: yaml
  label: 360Learning Custom Fields API
  slug: 360learning-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-custom-fields-api-openapi.yml
- filename: 360learning-custom-links-api-openapi.yml
  format: yaml
  label: 360Learning Custom Links API
  slug: 360learning-custom-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-custom-links-api-openapi.yml
- filename: 360learning-external-ids-api-openapi.yml
  format: yaml
  label: 360Learning External IDs API
  slug: 360learning-external-ids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-external-ids-api-openapi.yml
- filename: 360learning-groups-api-openapi.yml
  format: yaml
  label: 360Learning Groups API
  slug: 360learning-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-groups-api-openapi.yml
- filename: 360learning-integrations-api-openapi.yml
  format: yaml
  label: 360Learning Integrations API
  slug: 360learning-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-integrations-api-openapi.yml
- filename: 360learning-learning-needs-api-openapi.yml
  format: yaml
  label: 360Learning Learning Needs API
  slug: 360learning-learning-needs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-learning-needs-api-openapi.yml
- filename: 360learning-operations-api-openapi.yml
  format: yaml
  label: 360Learning Operations API
  slug: 360learning-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-operations-api-openapi.yml
- filename: 360learning-paths-api-openapi.yml
  format: yaml
  label: 360Learning Paths API
  slug: 360learning-paths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-paths-api-openapi.yml
- filename: 360learning-projects-api-openapi.yml
  format: yaml
  label: 360Learning Projects API
  slug: 360learning-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-projects-api-openapi.yml
- filename: 360learning-skills-api-openapi.yml
  format: yaml
  label: 360Learning Skills API
  slug: 360learning-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-skills-api-openapi.yml
- filename: 360learning-subscriptions-api-openapi.yml
  format: yaml
  label: 360Learning Subscriptions API
  slug: 360learning-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-subscriptions-api-openapi.yml
- filename: 360learning-tags-api-openapi.yml
  format: yaml
  label: 360Learning Tags API
  slug: 360learning-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-tags-api-openapi.yml
- filename: 360learning-users-api-openapi.yml
  format: yaml
  label: 360Learning Users API
  slug: 360learning-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: 360learning.com
  spf: true
hosts:
- cert_expires: Aug 30 15:15:03 2026 GMT
  host: app.360learning.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: app.us.360learning.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 360Learning Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 360Learning, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: 360Learning
provider_slug: 360learning
slug: 360learning-domain-security
source_filename: 360learning-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.360learning.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 15:15:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.us.360learning.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 360learning.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/security/360learning-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- EdTech
- Learning Management System
- E-Learning
- Training
- Collaborative Learning
- HR Tech
- Skills
---
