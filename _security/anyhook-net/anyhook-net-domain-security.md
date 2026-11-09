---
api_specs:
- filename: anyhook-net-anyhook-api-api-openapi.yml
  format: yaml
  label: AnyHook AnyHook API
  slug: anyhook-net-anyhook-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anyhook-net/openapi/anyhook-net-anyhook-api-api-openapi.yml
- filename: anyhook-net-api-keys-api-openapi.yml
  format: yaml
  label: AnyHook Api Keys API
  slug: anyhook-net-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anyhook-net/openapi/anyhook-net-api-keys-api-openapi.yml
- filename: anyhook-net-apps-api-openapi.yml
  format: yaml
  label: AnyHook Apps API
  slug: anyhook-net-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anyhook-net/openapi/anyhook-net-apps-api-openapi.yml
- filename: anyhook-net-claim-api-openapi.yml
  format: yaml
  label: AnyHook Claim API
  slug: anyhook-net-claim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anyhook-net/openapi/anyhook-net-claim-api-openapi.yml
- filename: anyhook-net-connect-api-openapi.yml
  format: yaml
  label: AnyHook Connect API
  slug: anyhook-net-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anyhook-net/openapi/anyhook-net-connect-api-openapi.yml
- filename: anyhook-net-events-api-openapi.yml
  format: yaml
  label: AnyHook Events API
  slug: anyhook-net-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anyhook-net/openapi/anyhook-net-events-api-openapi.yml
- filename: anyhook-net-quickstart-api-openapi.yml
  format: yaml
  label: AnyHook Quickstart API
  slug: anyhook-net-quickstart-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anyhook-net/openapi/anyhook-net-quickstart-api-openapi.yml
- filename: anyhook-net-usage-api-openapi.yml
  format: yaml
  label: AnyHook Usage API
  slug: anyhook-net-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anyhook-net/openapi/anyhook-net-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anyhook.net
  spf: true
hosts:
- cert_expires: Jan 11 11:42:00 2027 GMT
  host: anyhook.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anyhook Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AnyHook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AnyHook
provider_slug: anyhook-net
slug: anyhook-net-domain-security
source_filename: anyhook-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anyhook.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 11:42:00 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: anyhook.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/anyhook-net/security/anyhook-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Webhook
- Integration
- Reliability
- Developer Tools
- event-replay
---
