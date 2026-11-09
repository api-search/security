---
api_specs:
- filename: domeneschluse-no-app-api-openapi.yml
  format: yaml
  label: Domeneschluse App API
  slug: domeneschluse-no-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domeneschluse-no/openapi/domeneschluse-no-app-api-openapi.yml
- filename: domeneschluse-no-healthz-api-openapi.yml
  format: yaml
  label: Domeneschluse Healthz API
  slug: domeneschluse-no-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domeneschluse-no/openapi/domeneschluse-no-healthz-api-openapi.yml
- filename: domeneschluse-no-historikk-api-openapi.yml
  format: yaml
  label: Domeneschluse Historikk API
  slug: domeneschluse-no-historikk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domeneschluse-no/openapi/domeneschluse-no-historikk-api-openapi.yml
- filename: domeneschluse-no-koble-til-api-openapi.yml
  format: yaml
  label: Domeneschluse Koble Til API
  slug: domeneschluse-no-koble-til-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domeneschluse-no/openapi/domeneschluse-no-koble-til-api-openapi.yml
- filename: domeneschluse-no-mcp-api-openapi.yml
  format: yaml
  label: Domeneschluse MCP API
  slug: domeneschluse-no-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domeneschluse-no/openapi/domeneschluse-no-mcp-api-openapi.yml
- filename: domeneschluse-no-samtykke-api-openapi.yml
  format: yaml
  label: Domeneschluse Samtykke API
  slug: domeneschluse-no-samtykke-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domeneschluse-no/openapi/domeneschluse-no-samtykke-api-openapi.yml
- filename: domeneschluse-no-well-known-api-openapi.yml
  format: yaml
  label: Domeneschluse .well Known API
  slug: domeneschluse-no-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domeneschluse-no/openapi/domeneschluse-no-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: domeneschluse.no
  spf: true
hosts:
- cert_expires: Dec 15 07:28:48 2026 GMT
  host: domeneschluse.no
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Domeneschluse No Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Domeneschluse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Domeneschluse
provider_slug: domeneschluse-no
slug: domeneschluse-no-domain-security
source_filename: domeneschluse-no-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domeneschluse.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 07:28:48 2026 GMT\n  hsts: null\ndomains:\n- domain: domeneschluse.no\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/domeneschluse-no/security/domeneschluse-no-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Email
- Artificial Intelligence
- MCP
- Open Source
- Privacy
---
