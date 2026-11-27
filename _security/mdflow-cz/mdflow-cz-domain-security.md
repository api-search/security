---
api_specs:
- filename: mdflow-cz-documents-api-openapi.yml
  format: yaml
  label: MDflow Documents API
  slug: mdflow-cz-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdflow-cz/openapi/mdflow-cz-documents-api-openapi.yml
- filename: mdflow-cz-folders-api-openapi.yml
  format: yaml
  label: MDflow Folders API
  slug: mdflow-cz-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdflow-cz/openapi/mdflow-cz-folders-api-openapi.yml
- filename: mdflow-cz-team-documents-api-openapi.yml
  format: yaml
  label: MDflow Team documents API
  slug: mdflow-cz-team-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdflow-cz/openapi/mdflow-cz-team-documents-api-openapi.yml
- filename: mdflow-cz-team-folders-api-openapi.yml
  format: yaml
  label: MDflow Team folders API
  slug: mdflow-cz-team-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdflow-cz/openapi/mdflow-cz-team-folders-api-openapi.yml
- filename: mdflow-cz-team-workspaces-api-openapi.yml
  format: yaml
  label: MDflow Team workspaces API
  slug: mdflow-cz-team-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdflow-cz/openapi/mdflow-cz-team-workspaces-api-openapi.yml
- filename: mdflow-cz-workspaces-api-openapi.yml
  format: yaml
  label: MDflow Workspaces API
  slug: mdflow-cz-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdflow-cz/openapi/mdflow-cz-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mdflow.cz
  spf: true
hosts:
- cert_expires: Dec 24 17:45:07 2026 GMT
  host: mdflow.cz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MDflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MDflow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: MDflow
provider_slug: mdflow-cz
slug: mdflow-cz-domain-security
source_filename: mdflow-cz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mdflow.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 17:45:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mdflow.cz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mdflow-cz/security/mdflow-cz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Markdown editor
- Knowledge Base
- AI Agents
- Web clipper
---
