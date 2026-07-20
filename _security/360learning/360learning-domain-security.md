---
api_specs:
- filename: 360learning-core-api.json
  format: json
  label: 360Learning Core API v2
  slug: 360learning-core-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-core-api.json
- filename: 360learning-bulk-api.json
  format: json
  label: 360Learning Bulk API v2
  slug: 360learning-bulk-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-bulk-api.json
- filename: 360learning-webhook-api.json
  format: json
  label: 360Learning Webhook API v2
  slug: 360learning-webhook-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-webhook-api.json
- filename: 360learning-plugin-api.json
  format: json
  label: 360Learning Plugin API v2
  slug: 360learning-plugin-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-plugin-api.json
- filename: 360learning-user-authorized-api.json
  format: json
  label: 360Learning User Authorized API v2
  slug: 360learning-user-authorized-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-user-authorized-api.json
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
- Edtech
- Learning Management System
- E-Learning
- Training
- Collaborative Learning
- HR Tech
- Skills
- API
---
