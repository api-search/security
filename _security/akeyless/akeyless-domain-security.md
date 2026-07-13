---
api_specs:
- filename: akeyless-akeyless-api-openapi.yml
  format: yaml
  label: Akeyless REST API
  slug: akeyless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeyless/refs/heads/main/openapi/akeyless-akeyless-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: akeyless.io
  spf: true
hosts:
- cert_expires: Aug 18 09:00:31 2026 GMT
  host: www.akeyless.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 17:10:38 2026 GMT
  host: docs.akeyless.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: api.akeyless.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akeyless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akeyless, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Akeyless
provider_slug: akeyless
slug: akeyless-domain-security
source_filename: akeyless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.akeyless.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 09:00:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.akeyless.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 17:10:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.akeyless.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: akeyless.io\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akeyless/refs/heads/main/security/akeyless-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Secrets Management
- Zero Trust
- Cloud Security
- Identity Security
- Machine Identity
- Certificate Management
- PKI
- KMS
- Encryption
- SSH Access
- Dynamic Secrets
- Privileged Access Management
- DevSecOps
---
