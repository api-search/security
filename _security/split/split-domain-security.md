---
api_specs:
- filename: split-admin-api-openapi.yml
  format: yaml
  label: Split Admin API
  slug: split-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/split/refs/heads/main/openapi/split-admin-api-openapi.yml
- filename: split-feature-flag-api-openapi.yml
  format: yaml
  label: Split Feature Flag API
  slug: split-feature-flag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/split/refs/heads/main/openapi/split-feature-flag-api-openapi.yml
- filename: split-evaluator-api-openapi.yml
  format: yaml
  label: Split Evaluator API
  slug: split-evaluator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/split/refs/heads/main/openapi/split-evaluator-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "aws.amazon.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: split.io
  spf: true
hosts:
- cert_expires: Sep  7 11:00:24 2026 GMT
  host: docs.split.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 07:14:48 2026 GMT
  host: www.split.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 13:31:12 2026 GMT
  host: help.split.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Split Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Split, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Split
provider_slug: split
slug: split-domain-security
source_filename: split-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.split.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 11:00:24 2026 GMT\n  hsts: null\n- host: www.split.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 07:14:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.split.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 13:31:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: split.io\n  dnssec: true\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"aws.amazon.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/split/refs/heads/main/security/split-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Experimentation
- Feature Flags
- Feature Management
- Rollouts
- SDKs
---
