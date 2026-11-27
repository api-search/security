---
api_specs:
- filename: mzizi-dev-architecture-api-openapi.yml
  format: yaml
  label: Mzizi Architecture API
  slug: mzizi-dev-architecture-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mzizi-dev/openapi/mzizi-dev-architecture-api-openapi.yml
- filename: mzizi-dev-brand-api-openapi.yml
  format: yaml
  label: Mzizi Brand API
  slug: mzizi-dev-brand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mzizi-dev/openapi/mzizi-dev-brand-api-openapi.yml
- filename: mzizi-dev-content-api-openapi.yml
  format: yaml
  label: Mzizi Content API
  slug: mzizi-dev-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mzizi-dev/openapi/mzizi-dev-content-api-openapi.yml
- filename: mzizi-dev-discovery-api-openapi.yml
  format: yaml
  label: Mzizi Discovery API
  slug: mzizi-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mzizi-dev/openapi/mzizi-dev-discovery-api-openapi.yml
- filename: mzizi-dev-mcp-api-openapi.yml
  format: yaml
  label: Mzizi MCP API
  slug: mzizi-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mzizi-dev/openapi/mzizi-dev-mcp-api-openapi.yml
- filename: mzizi-dev-registry-api-openapi.yml
  format: yaml
  label: Mzizi Registry API
  slug: mzizi-dev-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mzizi-dev/openapi/mzizi-dev-registry-api-openapi.yml
- filename: mzizi-dev-ubuntu-api-openapi.yml
  format: yaml
  label: Mzizi Ubuntu API
  slug: mzizi-dev-ubuntu-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mzizi-dev/openapi/mzizi-dev-ubuntu-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mzizi.dev
  spf: false
hosts:
- cert_expires: Feb 16 09:20:39 2027 GMT
  host: mzizi.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mzizi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mzizi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Mzizi
provider_slug: mzizi-dev
slug: mzizi-dev-domain-security
source_filename: mzizi-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mzizi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 09:20:39 2027 GMT\n  hsts: false\ndomains:\n- domain: mzizi.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mzizi-dev/security/mzizi-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Programming Language
- Open Source
- Rust
- Compilers
- UI Components
---
