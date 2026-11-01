---
api_specs:
- filename: jobflow-openapi.json
  format: json
  label: Jobflow API
  slug: jobflow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kulalabs-ch/openapi/_original/jobflow-openapi.json
- filename: pazair-openapi.json
  format: json
  label: PazAIr API
  slug: pazair-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kulalabs-ch/openapi/_original/pazair-openapi.json
- filename: agents-openapi.json
  format: json
  label: Agents API
  slug: agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kulalabs-ch/openapi/_original/agents-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kulalabs.ch
  spf: true
hosts:
- cert_expires: Jan  2 17:49:52 2027 GMT
  host: kulalabs.ch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kulalabs Ch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for kulalabs-ch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: kulalabs-ch
provider_slug: kulalabs-ch
slug: kulalabs-ch-domain-security
source_filename: kulalabs-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kulalabs.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 17:49:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kulalabs.ch\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kulalabs-ch/security/kulalabs-ch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Software
- AI
- Water
- Switzerland
- Automation
---
