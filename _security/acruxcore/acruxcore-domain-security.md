---
api_specs:
- filename: acruxcore-openapi-generated.yml
  format: yaml
  label: Acrux Core API
  slug: acruxcore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acruxcore/refs/heads/main/openapi/_ae-authored/acruxcore-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acruxcore.com
  spf: true
hosts:
- cert_expires: Dec  9 18:39:44 2026 GMT
  host: acruxcore.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Acruxcore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acrux Core, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acrux Core
provider_slug: acruxcore
slug: acruxcore-domain-security
source_filename: acruxcore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acruxcore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 18:39:44 2026 GMT\n  hsts: false\ndomains:\n- domain: acruxcore.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acruxcore/refs/heads/main/security/acruxcore-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- LLMOps
- OpenSource
- Platform
- Engineering
- AI
---
