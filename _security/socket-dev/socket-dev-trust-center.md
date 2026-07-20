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
certifications:
- SOC 2 Type I
description: Socket's public trust / compliance posture. Socket announced SOC 2 Type I compliance, verifying its security controls against the AICPA Trust Services Criteria, and monitors internal controls continuously via an automated compliance platform. A key privacy property is that Socket is designed to operate without analyzing, uploading, or sharing customer source code. The trust page (socket.dev/legal/trust) blocks automated fetches (HTTP 403) so the certification set is captured from the public SOC 2 announcement.
kind: trust-center
layout: security
name: Socket Dev Trust Center
name_suffix: Trust Center
overview: Socket maintains a public trust center documenting SOC 2 Type I compliance.
provider_name: Socket
provider_slug: socket-dev
slug: socket-dev-trust-center
source_filename: socket-dev-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nprobe: true\nurl: https://socket.dev/legal/trust\nsource: https://socket.dev/blog/announcing-soc-2-type-i-compliance\ndescription: >-\n  Socket's public trust / compliance posture. Socket announced SOC 2 Type I compliance,\n  verifying its security controls against the AICPA Trust Services Criteria, and monitors\n  internal controls continuously via an automated compliance platform. A key privacy\n  property is that Socket is designed to operate without analyzing, uploading, or sharing\n  customer source code. The trust page (socket.dev/legal/trust) blocks automated fetches\n  (HTTP 403) so the certification set is captured from the public SOC 2 announcement.\ncertifications:\n  - name: SOC 2 Type I\n    framework: AICPA Trust Services Criteria\n    source: https://socket.dev/blog/announcing-soc-2-type-i-compliance\n    status: announced\nprivacy:\n  source_code_handling: Socket does not require analyzing, uploading, or sharing source\
  \ code.\nevidence:\n  - source: https://socket.dev/blog/announcing-soc-2-type-i-compliance\n    keywords: [soc 2, aicpa, trust services, compliance]\n  - source: https://socket.dev/legal/trust\n    note: linked as TrustCenter in apis.yml; returns 403 to automated clients\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/security/socket-dev-trust-center.yml
summary_line: SOC 2 Type I
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
trust_url: https://socket.dev/legal/trust
---
