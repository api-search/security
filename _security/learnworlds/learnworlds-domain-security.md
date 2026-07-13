---
api_specs:
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Users API
  slug: learnworlds-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Courses API
  slug: learnworlds-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Enrollments API
  slug: learnworlds-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Payments API
  slug: learnworlds-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Progress API
  slug: learnworlds-progress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Tags API
  slug: learnworlds-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Webhooks API
  slug: learnworlds-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: learnworlds.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: learnworlds.dev
  spf: false
hosts:
- cert_expires: Oct  7 07:31:15 2026 GMT
  host: www.learnworlds.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 11:26:08 2026 GMT
  host: www.learnworlds.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Learnworlds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LearnWorlds, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LearnWorlds
provider_slug: learnworlds
slug: learnworlds-domain-security
source_filename: learnworlds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.learnworlds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 07:31:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.learnworlds.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 11:26:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: learnworlds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: learnworlds.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/security/learnworlds-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Online Courses
- LMS
- eLearning
- Education
- Course Platform
- Creator Economy
---
