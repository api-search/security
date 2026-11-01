---
api_specs:
- filename: adaptris-adapter-api-openapi.yml
  format: yaml
  label: Adaptris /adapter API
  slug: adaptris-adapter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adaptris/openapi/adaptris-adapter-api-openapi.yml
- filename: adaptris-adapter-component-checker-api-openapi.yml
  format: yaml
  label: Adaptris /adapter/component Checker API
  slug: adaptris-adapter-component-checker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adaptris/openapi/adaptris-adapter-component-checker-api-openapi.yml
- filename: adaptris-adapter-failed-messages-api-openapi.yml
  format: yaml
  label: Adaptris /adapter/failed Messages API
  slug: adaptris-adapter-failed-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adaptris/openapi/adaptris-adapter-failed-messages-api-openapi.yml
- filename: adaptris-adapter-metrics-api-openapi.yml
  format: yaml
  label: Adaptris /adapter/metrics API
  slug: adaptris-adapter-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adaptris/openapi/adaptris-adapter-metrics-api-openapi.yml
- filename: adaptris-adapter-platform-api-openapi.yml
  format: yaml
  label: Adaptris /adapter/platform API
  slug: adaptris-adapter-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adaptris/openapi/adaptris-adapter-platform-api-openapi.yml
- filename: adaptris-channel-api-openapi.yml
  format: yaml
  label: Adaptris /channel API
  slug: adaptris-channel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adaptris/openapi/adaptris-channel-api-openapi.yml
- filename: adaptris-channel-failed-messages-api-openapi.yml
  format: yaml
  label: Adaptris /channel/failed Messages API
  slug: adaptris-channel-failed-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adaptris/openapi/adaptris-channel-failed-messages-api-openapi.yml
- filename: adaptris-channel-metrics-api-openapi.yml
  format: yaml
  label: Adaptris /channel/metrics API
  slug: adaptris-channel-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adaptris/openapi/adaptris-channel-metrics-api-openapi.yml
- filename: adaptris-deprecated-api-openapi.yml
  format: yaml
  label: Adaptris Deprecated API
  slug: adaptris-deprecated-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adaptris/openapi/adaptris-deprecated-api-openapi.yml
- filename: adaptris-workflow-api-openapi.yml
  format: yaml
  label: Adaptris /workflow API
  slug: adaptris-workflow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adaptris/openapi/adaptris-workflow-api-openapi.yml
- filename: adaptris-workflow-failed-messages-api-openapi.yml
  format: yaml
  label: Adaptris /workflow/failed Messages API
  slug: adaptris-workflow-failed-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adaptris/openapi/adaptris-workflow-failed-messages-api-openapi.yml
- filename: adaptris-workflow-metrics-api-openapi.yml
  format: yaml
  label: Adaptris /workflow/metrics API
  slug: adaptris-workflow-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adaptris/openapi/adaptris-workflow-metrics-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adaptris.com
  spf: true
hosts:
- cert_expires: Nov 26 16:18:46 2026 GMT
  host: adaptris.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adaptris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adaptris, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Adaptris
provider_slug: adaptris
slug: adaptris-domain-security
source_filename: adaptris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adaptris.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 16:18:46 2026 GMT\n  hsts: false\ndomains:\n- domain: adaptris.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/adaptris/security/adaptris-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Integration
- Messaging
- Cloud
---
