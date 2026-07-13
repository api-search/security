---
api_specs:
- filename: socket-packages-api-openapi.yml
  format: yaml
  label: Socket Packages API
  slug: socket-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-packages-api-openapi.yml
- filename: socket-full-scans-api-openapi.yml
  format: yaml
  label: Socket Full Scans API
  slug: socket-full-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-full-scans-api-openapi.yml
- filename: socket-diff-scans-api-openapi.yml
  format: yaml
  label: Socket Diff Scans API
  slug: socket-diff-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-diff-scans-api-openapi.yml
- filename: socket-alerts-api-openapi.yml
  format: yaml
  label: Socket Alerts API
  slug: socket-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-alerts-api-openapi.yml
- filename: socket-triage-api-openapi.yml
  format: yaml
  label: Socket Triage API
  slug: socket-triage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-triage-api-openapi.yml
- filename: socket-repos-api-openapi.yml
  format: yaml
  label: Socket Repos API
  slug: socket-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-repos-api-openapi.yml
- filename: socket-org-settings-api-openapi.yml
  format: yaml
  label: Socket Organization Settings API
  slug: socket-org-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-org-settings-api-openapi.yml
- filename: socket-webhooks-api-openapi.yml
  format: yaml
  label: Socket Webhooks API
  slug: socket-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-webhooks-api-openapi.yml
- filename: socket-threat-feed-api-openapi.yml
  format: yaml
  label: Socket Threat Feed API
  slug: socket-threat-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-threat-feed-api-openapi.yml
- filename: socket-fixes-api-openapi.yml
  format: yaml
  label: Socket Fixes API
  slug: socket-fixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-fixes-api-openapi.yml
- filename: socket-dependencies-api-openapi.yml
  format: yaml
  label: Socket Dependencies API
  slug: socket-dependencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dependencies-api-openapi.yml
- filename: socket-api-tokens-api-openapi.yml
  format: yaml
  label: Socket API Tokens API
  slug: socket-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-api-tokens-api-openapi.yml
- filename: socket-audit-log-api-openapi.yml
  format: yaml
  label: Socket Audit Log API
  slug: socket-audit-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-audit-log-api-openapi.yml
- filename: socket-org-snapshots-api-openapi.yml
  format: yaml
  label: Socket Organization Snapshots API
  slug: socket-org-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-org-snapshots-api-openapi.yml
- filename: socket-metadata-api-openapi.yml
  format: yaml
  label: Socket Metadata API
  slug: socket-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-metadata-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: socket.dev
  spf: true
hosts:
- cert_expires: Aug 15 19:56:03 2026 GMT
  host: socket.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 00:20:47 2026 GMT
  host: docs.socket.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 19:58:16 2026 GMT
  host: api.socket.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Socket Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Socket, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Socket
provider_slug: socket-dev
slug: socket-dev-domain-security
source_filename: socket-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: socket.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 19:56:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.socket.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 00:20:47 2026 GMT\n  hsts: null\n- host: api.socket.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 19:58:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: socket.dev\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/security/socket-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Supply Chain Security
- Open Source Security
- Software Composition Analysis
- SCA
- Malware Detection
- Dependency Scanning
- SBOM
- npm
- PyPI
- Go
- Maven
- Cargo
- NuGet
- RubyGems
- Developer Security
---
