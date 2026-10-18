---
api_specs:
- filename: coincover-backup-api-openapi.yml
  format: yaml
  label: Coincover Backup API
  slug: coincover-backup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coincover/refs/heads/main/openapi/coincover-backup-api-openapi.yml
- filename: coincover-backups-api-openapi.yml
  format: yaml
  label: Coincover Backups API
  slug: coincover-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coincover/refs/heads/main/openapi/coincover-backups-api-openapi.yml
- filename: coincover-key-api-openapi.yml
  format: yaml
  label: Coincover Key API
  slug: coincover-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coincover/refs/heads/main/openapi/coincover-key-api-openapi.yml
- filename: coincover-keys-api-openapi.yml
  format: yaml
  label: Coincover Keys API
  slug: coincover-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coincover/refs/heads/main/openapi/coincover-keys-api-openapi.yml
- filename: coincover-partner-api-openapi.yml
  format: yaml
  label: Coincover Partner API
  slug: coincover-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coincover/refs/heads/main/openapi/coincover-partner-api-openapi.yml
- filename: coincover-secure-api-openapi.yml
  format: yaml
  label: Coincover Secure API
  slug: coincover-secure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coincover/refs/heads/main/openapi/coincover-secure-api-openapi.yml
- filename: coincover-verification-api-openapi.yml
  format: yaml
  label: Coincover Verification API
  slug: coincover-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coincover/refs/heads/main/openapi/coincover-verification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coincover.com
  spf: true
hosts:
- cert_expires: Nov 21 19:48:09 2026 GMT
  host: www.coincover.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coincover Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coincover, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coincover
provider_slug: coincover
slug: coincover-domain-security
source_filename: coincover-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coincover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 19:48:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coincover.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coincover/refs/heads/main/security/coincover-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Security
- Recovery
- Fintech
---
