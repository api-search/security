---
api_specs:
- filename: toloka-assignments-api-openapi.yml
  format: yaml
  label: Toloka Assignments API
  slug: toloka-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-assignments-api-openapi.yml
- filename: toloka-attachments-api-openapi.yml
  format: yaml
  label: Toloka Attachments API
  slug: toloka-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-attachments-api-openapi.yml
- filename: toloka-operations-api-openapi.yml
  format: yaml
  label: Toloka Operations API
  slug: toloka-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-operations-api-openapi.yml
- filename: toloka-pools-api-openapi.yml
  format: yaml
  label: Toloka Pools API
  slug: toloka-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-pools-api-openapi.yml
- filename: toloka-projects-api-openapi.yml
  format: yaml
  label: Toloka Projects API
  slug: toloka-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-projects-api-openapi.yml
- filename: toloka-skills-api-openapi.yml
  format: yaml
  label: Toloka Skills API
  slug: toloka-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-skills-api-openapi.yml
- filename: toloka-task-suites-api-openapi.yml
  format: yaml
  label: Toloka Task Suites API
  slug: toloka-task-suites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-task-suites-api-openapi.yml
- filename: toloka-tasks-api-openapi.yml
  format: yaml
  label: Toloka Tasks API
  slug: toloka-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-tasks-api-openapi.yml
- filename: toloka-training-api-openapi.yml
  format: yaml
  label: Toloka Training API
  slug: toloka-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-training-api-openapi.yml
- filename: toloka-user-bonuses-api-openapi.yml
  format: yaml
  label: Toloka User Bonuses API
  slug: toloka-user-bonuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-user-bonuses-api-openapi.yml
- filename: toloka-user-restrictions-api-openapi.yml
  format: yaml
  label: Toloka User Restrictions API
  slug: toloka-user-restrictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-user-restrictions-api-openapi.yml
- filename: toloka-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Toloka Webhook Subscriptions API
  slug: toloka-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-webhook-subscriptions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: toloka.ai
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: toloka.dev
  spf: false
hosts:
- cert_expires: Jul 27 04:44:40 2026 GMT
  host: toloka.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.toloka.ai
  https: false
- cert_expires: Sep 18 06:19:34 2026 GMT
  host: toloka.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Toloka Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toloka, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Toloka
provider_slug: toloka
slug: toloka-domain-security
source_filename: toloka-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: toloka.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 27 04:44:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.toloka.ai\n  https: false\n- host: toloka.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 06:19:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: toloka.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: toloka.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/security/toloka-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Labeling
- Crowdsourcing
- Human-in-the-Loop
- Training Data
- AI
---
