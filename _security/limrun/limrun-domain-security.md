---
api_specs:
- filename: limrun-analytics-api-openapi.yml
  format: yaml
  label: Limrun Analytics API
  slug: limrun-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/limrun/refs/heads/main/openapi/limrun-analytics-api-openapi.yml
- filename: limrun-android-instances-api-openapi.yml
  format: yaml
  label: Limrun Android Instances API
  slug: limrun-android-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/limrun/refs/heads/main/openapi/limrun-android-instances-api-openapi.yml
- filename: limrun-assets-api-openapi.yml
  format: yaml
  label: Limrun Assets API
  slug: limrun-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/limrun/refs/heads/main/openapi/limrun-assets-api-openapi.yml
- filename: limrun-downloads-api-openapi.yml
  format: yaml
  label: Limrun Downloads API
  slug: limrun-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/limrun/refs/heads/main/openapi/limrun-downloads-api-openapi.yml
- filename: limrun-gradle-instances-api-openapi.yml
  format: yaml
  label: Limrun Gradle Instances API
  slug: limrun-gradle-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/limrun/refs/heads/main/openapi/limrun-gradle-instances-api-openapi.yml
- filename: limrun-ios-instances-api-openapi.yml
  format: yaml
  label: Limrun Ios Instances API
  slug: limrun-ios-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/limrun/refs/heads/main/openapi/limrun-ios-instances-api-openapi.yml
- filename: limrun-xcode-instances-api-openapi.yml
  format: yaml
  label: Limrun Xcode Instances API
  slug: limrun-xcode-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/limrun/refs/heads/main/openapi/limrun-xcode-instances-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lim.run
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: limrun.com
  spf: true
hosts:
- cert_expires: Aug 21 15:46:32 2026 GMT
  host: lim.run
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 20:19:13 2026 GMT
  host: docs.limrun.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 20:19:13 2026 GMT
  host: api.limrun.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Limrun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Limrun, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Limrun
provider_slug: limrun
slug: limrun-domain-security
source_filename: limrun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lim.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 15:46:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.limrun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 20:19:13 2026 GMT\n  hsts: false\n- host: api.limrun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 20:19:13 2026 GMT\n  hsts: null\ndomains:\n- domain: lim.run\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: limrun.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/limrun/refs/heads/main/security/limrun-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobile
- iOS
- Android
- Simulators
- Emulators
- Cloud Infrastructure
- Continuous Integration
- Developer Tools
- Testing
- Agents
- MCP
- Sandboxes
- Xcode
---
