---
api_specs:
- filename: anchorregistry-ai-account-api-openapi.yml
  format: yaml
  label: AnchorRegistry Account API
  slug: anchorregistry-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchorregistry-ai/openapi/anchorregistry-ai-account-api-openapi.yml
- filename: anchorregistry-ai-discovery-api-openapi.yml
  format: yaml
  label: AnchorRegistry Discovery API
  slug: anchorregistry-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchorregistry-ai/openapi/anchorregistry-ai-discovery-api-openapi.yml
- filename: anchorregistry-ai-register-api-openapi.yml
  format: yaml
  label: AnchorRegistry Register API
  slug: anchorregistry-ai-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchorregistry-ai/openapi/anchorregistry-ai-register-api-openapi.yml
- filename: anchorregistry-ai-system-api-openapi.yml
  format: yaml
  label: AnchorRegistry System API
  slug: anchorregistry-ai-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchorregistry-ai/openapi/anchorregistry-ai-system-api-openapi.yml
- filename: anchorregistry-ai-verify-api-openapi.yml
  format: yaml
  label: AnchorRegistry Verify API
  slug: anchorregistry-ai-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchorregistry-ai/openapi/anchorregistry-ai-verify-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anchorregistry.ai
  spf: false
hosts:
- cert_expires: Jan 20 15:58:44 2027 GMT
  host: anchorregistry.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AnchorRegistry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AnchorRegistry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: AnchorRegistry
provider_slug: anchorregistry-ai
slug: anchorregistry-ai-domain-security
source_filename: anchorregistry-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anchorregistry.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 15:58:44 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: anchorregistry.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/anchorregistry-ai/security/anchorregistry-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Provenance
- Onchain
- Artificial Intelligence
- Data
- Artifacts
---
