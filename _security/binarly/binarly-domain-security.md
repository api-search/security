---
api_specs:
- filename: binarly-assistant-api-openapi.yml
  format: yaml
  label: Binarly Assistant API
  slug: binarly-assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-assistant-api-openapi.yml
- filename: binarly-chart-api-openapi.yml
  format: yaml
  label: Binarly Chart API
  slug: binarly-chart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-chart-api-openapi.yml
- filename: binarly-customrules-api-openapi.yml
  format: yaml
  label: Binarly CustomRules API
  slug: binarly-customrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-customrules-api-openapi.yml
- filename: binarly-escalation-api-openapi.yml
  format: yaml
  label: Binarly Escalation API
  slug: binarly-escalation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-escalation-api-openapi.yml
- filename: binarly-file-api-openapi.yml
  format: yaml
  label: Binarly File API
  slug: binarly-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-file-api-openapi.yml
- filename: binarly-finding-api-openapi.yml
  format: yaml
  label: Binarly Finding API
  slug: binarly-finding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-finding-api-openapi.yml
- filename: binarly-grid-api-openapi.yml
  format: yaml
  label: Binarly Grid API
  slug: binarly-grid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-grid-api-openapi.yml
- filename: binarly-group-api-openapi.yml
  format: yaml
  label: Binarly Group API
  slug: binarly-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-group-api-openapi.yml
- filename: binarly-image-api-openapi.yml
  format: yaml
  label: Binarly Image API
  slug: binarly-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-image-api-openapi.yml
- filename: binarly-integration-api-openapi.yml
  format: yaml
  label: Binarly Integration API
  slug: binarly-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-integration-api-openapi.yml
- filename: binarly-notification-api-openapi.yml
  format: yaml
  label: Binarly Notification API
  slug: binarly-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-notification-api-openapi.yml
- filename: binarly-product-api-openapi.yml
  format: yaml
  label: Binarly Product API
  slug: binarly-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-product-api-openapi.yml
- filename: binarly-rolebinding-api-openapi.yml
  format: yaml
  label: Binarly RoleBinding API
  slug: binarly-rolebinding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-rolebinding-api-openapi.yml
- filename: binarly-scan-api-openapi.yml
  format: yaml
  label: Binarly Scan API
  slug: binarly-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-scan-api-openapi.yml
- filename: binarly-search-api-openapi.yml
  format: yaml
  label: Binarly Search API
  slug: binarly-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-search-api-openapi.yml
- filename: binarly-subscription-api-openapi.yml
  format: yaml
  label: Binarly Subscription API
  slug: binarly-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-subscription-api-openapi.yml
- filename: binarly-tempfile-api-openapi.yml
  format: yaml
  label: Binarly TempFile API
  slug: binarly-tempfile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-tempfile-api-openapi.yml
- filename: binarly-user-api-openapi.yml
  format: yaml
  label: Binarly User API
  slug: binarly-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-user-api-openapi.yml
- filename: binarly-userstorage-api-openapi.yml
  format: yaml
  label: Binarly UserStorage API
  slug: binarly-userstorage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-userstorage-api-openapi.yml
- filename: binarly-vulnerability-api-openapi.yml
  format: yaml
  label: Binarly Vulnerability API
  slug: binarly-vulnerability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/openapi/binarly-vulnerability-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: binarly.io
  spf: true
hosts:
- cert_expires: Aug 21 12:25:29 2026 GMT
  host: docs.binarly.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Binarly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Binarly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Binarly
provider_slug: binarly
slug: binarly-domain-security
source_filename: binarly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.binarly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 12:25:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: binarly.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/binarly/refs/heads/main/security/binarly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Firmware Security
- Supply Chain Security
- Vulnerability Management
- SBOM
- Binary Analysis
- Post-Quantum Cryptography
- UEFI
- DevSecOps
---
