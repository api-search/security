---
api_specs:
- filename: toloka-openapi.yml
  format: yaml
  label: Toloka Projects API
  slug: projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-openapi.yml
- filename: toloka-openapi.yml
  format: yaml
  label: Toloka Pools API
  slug: pools
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-openapi.yml
- filename: toloka-openapi.yml
  format: yaml
  label: Toloka Tasks & Task Suites API
  slug: tasks-task-suites
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-openapi.yml
- filename: toloka-openapi.yml
  format: yaml
  label: Toloka Assignments API
  slug: assignments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-openapi.yml
- filename: toloka-openapi.yml
  format: yaml
  label: Toloka Operations & Webhooks API
  slug: operations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toloka/refs/heads/main/openapi/toloka-openapi.yml
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
