---
api_specs:
- filename: honcho-dev-apps-api-openapi.yml
  format: yaml
  label: Honcho Apps API
  slug: honcho-dev-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honcho-dev/openapi/honcho-dev-apps-api-openapi.yml
- filename: honcho-dev-collections-api-openapi.yml
  format: yaml
  label: Honcho Collections API
  slug: honcho-dev-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honcho-dev/openapi/honcho-dev-collections-api-openapi.yml
- filename: honcho-dev-documents-api-openapi.yml
  format: yaml
  label: Honcho Documents API
  slug: honcho-dev-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honcho-dev/openapi/honcho-dev-documents-api-openapi.yml
- filename: honcho-dev-keys-api-openapi.yml
  format: yaml
  label: Honcho Keys API
  slug: honcho-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honcho-dev/openapi/honcho-dev-keys-api-openapi.yml
- filename: honcho-dev-messages-api-openapi.yml
  format: yaml
  label: Honcho Messages API
  slug: honcho-dev-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honcho-dev/openapi/honcho-dev-messages-api-openapi.yml
- filename: honcho-dev-metamessages-api-openapi.yml
  format: yaml
  label: Honcho Metamessages API
  slug: honcho-dev-metamessages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honcho-dev/openapi/honcho-dev-metamessages-api-openapi.yml
- filename: honcho-dev-sessions-api-openapi.yml
  format: yaml
  label: Honcho Sessions API
  slug: honcho-dev-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honcho-dev/openapi/honcho-dev-sessions-api-openapi.yml
- filename: honcho-dev-users-api-openapi.yml
  format: yaml
  label: Honcho Users API
  slug: honcho-dev-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honcho-dev/openapi/honcho-dev-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: honcho.dev
  spf: true
hosts:
- cert_expires: Dec 18 05:30:09 2026 GMT
  host: honcho.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Honcho Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Honcho, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Honcho
provider_slug: honcho-dev
slug: honcho-dev-domain-security
source_filename: honcho-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: honcho.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 05:30:09 2026 GMT\n  hsts: false\ndomains:\n- domain: honcho.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/honcho-dev/security/honcho-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Memory
- Open Source
- Agents
- Platform
---
