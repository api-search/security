---
api_specs:
- filename: emerge-tools-analysis-api-openapi.yml
  format: yaml
  label: Emerge Tools Analysis API
  slug: emerge-tools-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-analysis-api-openapi.yml
- filename: emerge-tools-apphistory-api-openapi.yml
  format: yaml
  label: Emerge Tools AppHistory API
  slug: emerge-tools-apphistory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-apphistory-api-openapi.yml
- filename: emerge-tools-builddetails-api-openapi.yml
  format: yaml
  label: Emerge Tools BuildDetails API
  slug: emerge-tools-builddetails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-builddetails-api-openapi.yml
- filename: emerge-tools-comment-api-openapi.yml
  format: yaml
  label: Emerge Tools Comment API
  slug: emerge-tools-comment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-comment-api-openapi.yml
- filename: emerge-tools-deadcode-api-openapi.yml
  format: yaml
  label: Emerge Tools DeadCode API
  slug: emerge-tools-deadcode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-deadcode-api-openapi.yml
- filename: emerge-tools-getperftest-api-openapi.yml
  format: yaml
  label: Emerge Tools GetPerfTest API
  slug: emerge-tools-getperftest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-getperftest-api-openapi.yml
- filename: emerge-tools-snapshots-api-openapi.yml
  format: yaml
  label: Emerge Tools Snapshots API
  slug: emerge-tools-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-snapshots-api-openapi.yml
- filename: emerge-tools-trace-api-openapi.yml
  format: yaml
  label: Emerge Tools Trace API
  slug: emerge-tools-trace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-trace-api-openapi.yml
- filename: emerge-tools-upload-api-openapi.yml
  format: yaml
  label: Emerge Tools Upload API
  slug: emerge-tools-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-upload-api-openapi.yml
- filename: emerge-tools-uploadfromlink-api-openapi.yml
  format: yaml
  label: Emerge Tools UploadFromLink API
  slug: emerge-tools-uploadfromlink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/openapi/emerge-tools-uploadfromlink-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: emergetools.com
  spf: true
hosts:
- cert_expires: Oct 11 14:01:27 2026 GMT
  host: emergetools.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 14:01:27 2026 GMT
  host: api.emergetools.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emerge Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emerge Tools, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Emerge Tools
provider_slug: emerge-tools
slug: emerge-tools-domain-security
source_filename: emerge-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emergetools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 14:01:27 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.emergetools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 14:01:27 2026 GMT\n  hsts: null\ndomains:\n- domain: emergetools.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emerge-tools/refs/heads/main/security/emerge-tools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- B2B
- Mobile
- Developer Tools
- App Performance
- Testing
- iOS
- Android
- DevOps
---
