---
api_specs:
- filename: vertex-documents-api-openapi.yml
  format: yaml
  label: Vertex Documents API
  slug: vertex-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertex/refs/heads/main/openapi/vertex-documents-api-openapi.yml
- filename: vertex-problems-api-openapi.yml
  format: yaml
  label: Vertex Problems API
  slug: vertex-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertex/refs/heads/main/openapi/vertex-problems-api-openapi.yml
- filename: vertex-project-api-openapi.yml
  format: yaml
  label: Vertex Project API
  slug: vertex-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertex/refs/heads/main/openapi/vertex-project-api-openapi.yml
- filename: vertex-reports-api-openapi.yml
  format: yaml
  label: Vertex Reports API
  slug: vertex-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertex/refs/heads/main/openapi/vertex-reports-api-openapi.yml
- filename: vertex-schedules-api-openapi.yml
  format: yaml
  label: Vertex Schedules API
  slug: vertex-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertex/refs/heads/main/openapi/vertex-schedules-api-openapi.yml
- filename: vertex-templates-api-openapi.yml
  format: yaml
  label: Vertex Templates API
  slug: vertex-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertex/refs/heads/main/openapi/vertex-templates-api-openapi.yml
- filename: vertex-vertex-api-api-openapi.yml
  format: yaml
  label: Vertex Vertex API
  slug: vertex-vertex-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertex/refs/heads/main/openapi/vertex-vertex-api-api-openapi.yml
- filename: vertex-vertex-ws-api-openapi.yml
  format: yaml
  label: Vertex Vertex Ws API
  slug: vertex-vertex-ws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vertex/refs/heads/main/openapi/vertex-vertex-ws-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vertexinc.com
  spf: true
hosts:
- cert_expires: Dec 12 15:20:31 2026 GMT
  host: www.vertexinc.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vertex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vertex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vertex
provider_slug: vertex
slug: vertex-domain-security
source_filename: vertex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vertexinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 15:20:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: vertexinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vertex/refs/heads/main/security/vertex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Tax
- Compliance
- Automation
---
