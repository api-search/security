---
api_specs:
- filename: openbash-ai-changelog-api-openapi.yml
  format: yaml
  label: OpenBash AI Changelog API
  slug: openbash-ai-changelog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openbash-ai/openapi/openbash-ai-changelog-api-openapi.yml
- filename: openbash-ai-exec-api-openapi.yml
  format: yaml
  label: OpenBash AI Exec API
  slug: openbash-ai-exec-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openbash-ai/openapi/openbash-ai-exec-api-openapi.yml
- filename: openbash-ai-programs-api-openapi.yml
  format: yaml
  label: OpenBash AI Programs API
  slug: openbash-ai-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openbash-ai/openapi/openbash-ai-programs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openbash.ai
  spf: true
hosts:
- cert_expires: Jan 30 18:12:23 2027 GMT
  host: openbash.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenBash AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenBash AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OpenBash AI
provider_slug: openbash-ai
slug: openbash-ai-domain-security
source_filename: openbash-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openbash.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 18:12:23 2027 GMT\n  hsts: false\ndomains:\n- domain: openbash.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/openbash-ai/security/openbash-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data
- MCP
- Bash
- PrimaryData
---
