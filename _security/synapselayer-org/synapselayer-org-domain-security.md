---
api_specs:
- filename: synapselayer-org-discovery-api-openapi.yml
  format: yaml
  label: Synapse Layer Discovery API
  slug: synapselayer-org-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synapselayer-org/openapi/synapselayer-org-discovery-api-openapi.yml
- filename: synapselayer-org-memory-api-openapi.yml
  format: yaml
  label: Synapse Layer Memory API
  slug: synapselayer-org-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synapselayer-org/openapi/synapselayer-org-memory-api-openapi.yml
- filename: synapselayer-org-onboarding-api-openapi.yml
  format: yaml
  label: Synapse Layer Onboarding API
  slug: synapselayer-org-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synapselayer-org/openapi/synapselayer-org-onboarding-api-openapi.yml
- filename: synapselayer-org-operational-api-openapi.yml
  format: yaml
  label: Synapse Layer Operational API
  slug: synapselayer-org-operational-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synapselayer-org/openapi/synapselayer-org-operational-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: synapselayer.org
  spf: false
hosts:
- cert_expires: Feb 17 15:00:56 2027 GMT
  host: synapselayer.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Synapse Layer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synapse Layer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Synapse Layer
provider_slug: synapselayer-org
slug: synapselayer-org-domain-security
source_filename: synapselayer-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synapselayer.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 15:00:56 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: synapselayer.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/synapselayer-org/security/synapselayer-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- Memory
- Encryption
- MCP
- Trust
---
