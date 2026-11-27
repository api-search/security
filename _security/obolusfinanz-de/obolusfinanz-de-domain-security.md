---
api_specs:
- filename: obolusfinanz-de-mcp-api-openapi.yml
  format: yaml
  label: Obolus MCP API
  slug: obolusfinanz-de-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obolusfinanz-de/openapi/obolusfinanz-de-mcp-api-openapi.yml
- filename: obolusfinanz-de-resources-api-openapi.yml
  format: yaml
  label: Obolus Resources API
  slug: obolusfinanz-de-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obolusfinanz-de/openapi/obolusfinanz-de-resources-api-openapi.yml
- filename: obolusfinanz-de-tools-api-openapi.yml
  format: yaml
  label: Obolus Tools API
  slug: obolusfinanz-de-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obolusfinanz-de/openapi/obolusfinanz-de-tools-api-openapi.yml
- filename: obolusfinanz-de-open-api-api-openapi.yml
  format: yaml
  label: Obolus Open API
  slug: obolusfinanz-de-open-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obolusfinanz-de/openapi/obolusfinanz-de-open-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: obolusfinanz.de
  spf: true
hosts:
- cert_expires: Jan  5 20:04:58 2027 GMT
  host: obolusfinanz.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Obolus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Obolus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Obolus
provider_slug: obolusfinanz-de
slug: obolusfinanz-de-domain-security
source_filename: obolusfinanz-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: obolusfinanz.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 20:04:58 2027 GMT\n  hsts: false\ndomains:\n- domain: obolusfinanz.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/obolusfinanz-de/security/obolusfinanz-de-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Relocation
- Tools
- Salary
---
