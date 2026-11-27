---
api_specs:
- filename: configdirector-com-api-tokens-api-openapi.yml
  format: yaml
  label: ConfigDirector API tokens API
  slug: configdirector-com-api-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-api-tokens-api-openapi.yml
- filename: configdirector-com-configs-api-openapi.yml
  format: yaml
  label: ConfigDirector Configs API
  slug: configdirector-com-configs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-configs-api-openapi.yml
- filename: configdirector-com-discovery-api-openapi.yml
  format: yaml
  label: ConfigDirector Discovery API
  slug: configdirector-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-discovery-api-openapi.yml
- filename: configdirector-com-documentation-api-openapi.yml
  format: yaml
  label: ConfigDirector Documentation API
  slug: configdirector-com-documentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-documentation-api-openapi.yml
- filename: configdirector-com-environments-api-openapi.yml
  format: yaml
  label: ConfigDirector Environments API
  slug: configdirector-com-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-environments-api-openapi.yml
- filename: configdirector-com-projects-api-openapi.yml
  format: yaml
  label: ConfigDirector Projects API
  slug: configdirector-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-projects-api-openapi.yml
- filename: configdirector-com-scanned-repositories-api-openapi.yml
  format: yaml
  label: ConfigDirector Scanned repositories API
  slug: configdirector-com-scanned-repositories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-scanned-repositories-api-openapi.yml
- filename: configdirector-com-segments-api-openapi.yml
  format: yaml
  label: ConfigDirector Segments API
  slug: configdirector-com-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-segments-api-openapi.yml
- filename: configdirector-com-tags-api-openapi.yml
  format: yaml
  label: ConfigDirector Tags API
  slug: configdirector-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-tags-api-openapi.yml
- filename: configdirector-com-webhooks-api-openapi.yml
  format: yaml
  label: ConfigDirector Webhooks API
  slug: configdirector-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: configdirector.com
  spf: true
hosts:
- cert_expires: Jan 11 05:02:28 2027 GMT
  host: configdirector.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ConfigDirector Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConfigDirector, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ConfigDirector
provider_slug: configdirector-com
slug: configdirector-com-domain-security
source_filename: configdirector-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: configdirector.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 05:02:28 2027 GMT\n  hsts: false\ndomains:\n- domain: configdirector.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/configdirector-com/security/configdirector-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Feature Flags
- Remote Configuration
- Configuration Management
- Developer Tools
- OpenFeature
- SDK
- MCP
---
