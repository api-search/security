---
api_specs:
- filename: diagram-la-diagrams-api-openapi.yml
  format: yaml
  label: Diagram Diagrams API
  slug: diagram-la-diagrams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/diagram-la/openapi/diagram-la-diagrams-api-openapi.yml
- filename: diagram-la-projects-api-openapi.yml
  format: yaml
  label: Diagram Projects API
  slug: diagram-la-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/diagram-la/openapi/diagram-la-projects-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: diagram.la
  spf: true
hosts:
- cert_expires: Dec 27 19:16:18 2026 GMT
  host: diagram.la
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Diagram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diagram, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Diagram
provider_slug: diagram-la
slug: diagram-la-domain-security
source_filename: diagram-la-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: diagram.la\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 19:16:18 2026 GMT\n  hsts: false\ndomains:\n- domain: diagram.la\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/diagram-la/security/diagram-la-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Diagramming
- Visualization
- Artificial Intelligence
- MCP
- Collaboration
- Developer Tools
---
