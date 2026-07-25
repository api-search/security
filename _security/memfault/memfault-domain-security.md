---
api_specs:
- filename: memfault-organizations-api-openapi.yml
  format: yaml
  label: Memfault Organizations API
  slug: memfault-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-organizations-api-openapi.yml
- filename: memfault-projects-api-openapi.yml
  format: yaml
  label: Memfault Projects API
  slug: memfault-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-projects-api-openapi.yml
- filename: memfault-devices-api-openapi.yml
  format: yaml
  label: Memfault Devices API
  slug: memfault-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-devices-api-openapi.yml
- filename: memfault-issues-api-openapi.yml
  format: yaml
  label: Memfault Issues API
  slug: memfault-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-issues-api-openapi.yml
- filename: memfault-chunks-api-openapi.yml
  format: yaml
  label: Memfault Chunks Ingestion API
  slug: memfault-chunks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-chunks-api-openapi.yml
- filename: memfault-auth-api-openapi.yml
  format: yaml
  label: Memfault Auth API
  slug: memfault-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-auth-api-openapi.yml
- filename: memfault-chunks-api-openapi.yml
  format: yaml
  label: Memfault Chunks API
  slug: memfault-chunks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-chunks-api-openapi.yml
- filename: memfault-cohorts-api-openapi.yml
  format: yaml
  label: Memfault Cohorts API
  slug: memfault-cohorts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-cohorts-api-openapi.yml
- filename: memfault-deployments-api-openapi.yml
  format: yaml
  label: Memfault Deployments API
  slug: memfault-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-deployments-api-openapi.yml
- filename: memfault-devices-api-openapi.yml
  format: yaml
  label: Memfault Devices API
  slug: memfault-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-devices-api-openapi.yml
- filename: memfault-files-api-openapi.yml
  format: yaml
  label: Memfault Files API
  slug: memfault-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-files-api-openapi.yml
- filename: memfault-issues-api-openapi.yml
  format: yaml
  label: Memfault Issues API
  slug: memfault-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-issues-api-openapi.yml
- filename: memfault-organizations-api-openapi.yml
  format: yaml
  label: Memfault Organizations API
  slug: memfault-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-organizations-api-openapi.yml
- filename: memfault-projects-api-openapi.yml
  format: yaml
  label: Memfault Projects API
  slug: memfault-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-projects-api-openapi.yml
- filename: memfault-releases-api-openapi.yml
  format: yaml
  label: Memfault Releases API
  slug: memfault-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-releases-api-openapi.yml
- filename: memfault-software-api-openapi.yml
  format: yaml
  label: Memfault Software API
  slug: memfault-software-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/openapi/memfault-software-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: memfault.com
  spf: true
hosts:
- cert_expires: Sep 14 06:01:51 2026 GMT
  host: memfault.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 19:12:57 2026 GMT
  host: api-docs.memfault.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: api.memfault.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Memfault Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memfault, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Memfault
provider_slug: memfault
slug: memfault-domain-security
source_filename: memfault-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memfault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 06:01:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-docs.memfault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 19:12:57 2026 GMT\n  hsts: false\n- host: api.memfault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: memfault.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memfault/refs/heads/main/security/memfault-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Alerts
- Android
- Crash Reporting
- Device Management
- Embedded
- Embedded Linux
- Firmware
- IoT
- Logging
- MCU
- Metrics
- Observability
- OTA
- Reliability
---
