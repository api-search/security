---
api_specs:
- filename: attestari-ai-health-api-openapi.yml
  format: yaml
  label: Attestari Health API
  slug: attestari-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestari-ai/openapi/attestari-ai-health-api-openapi.yml
- filename: attestari-ai-manifest-api-openapi.yml
  format: yaml
  label: Attestari Manifest API
  slug: attestari-ai-manifest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestari-ai/openapi/attestari-ai-manifest-api-openapi.yml
- filename: attestari-ai-remote-api-openapi.yml
  format: yaml
  label: Attestari Remote API
  slug: attestari-ai-remote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestari-ai/openapi/attestari-ai-remote-api-openapi.yml
- filename: attestari-ai-verdict-api-openapi.yml
  format: yaml
  label: Attestari Verdict API
  slug: attestari-ai-verdict-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/attestari-ai/openapi/attestari-ai-verdict-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: attestari.ai
  spf: true
hosts:
- cert_expires: Dec  9 13:27:38 2026 GMT
  host: attestari.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Attestari Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Attestari, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Attestari
provider_slug: attestari-ai
slug: attestari-ai-domain-security
source_filename: attestari-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: attestari.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 13:27:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: attestari.ai\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/attestari-ai/security/attestari-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- MCP
- Security
- Compliance
- Open Source
---
