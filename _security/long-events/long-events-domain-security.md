---
api_specs:
- filename: long-events-discovery-api-openapi.yml
  format: yaml
  label: LONG Events Discovery API
  slug: long-events-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/long-events/openapi/long-events-discovery-api-openapi.yml
- filename: long-events-event-weeks-api-openapi.yml
  format: yaml
  label: LONG Events Event weeks API
  slug: long-events-event-weeks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/long-events/openapi/long-events-event-weeks-api-openapi.yml
- filename: long-events-events-and-artists-api-openapi.yml
  format: yaml
  label: LONG Events Events and artists API
  slug: long-events-events-and-artists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/long-events/openapi/long-events-events-and-artists-api-openapi.yml
- filename: long-events-long-5-api-openapi.yml
  format: yaml
  label: LONG Events LONG 5 API
  slug: long-events-long-5-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/long-events/openapi/long-events-long-5-api-openapi.yml
- filename: long-events-mcp-api-openapi.yml
  format: yaml
  label: LONG Events MCP API
  slug: long-events-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/long-events/openapi/long-events-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: long.events
  spf: true
hosts:
- cert_expires: Jan 23 13:29:36 2027 GMT
  host: long.events
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LONG Events Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LONG Events, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LONG Events
provider_slug: long-events
slug: long-events-domain-security
source_filename: long-events-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: long.events\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 13:29:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: long.events\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/long-events/security/long-events-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Event
- Artificial Intelligence
- Data
- MCP
- REST
---
