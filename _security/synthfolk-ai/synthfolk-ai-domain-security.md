---
api_specs:
- filename: synthfolk-ai-agents-api-openapi.yml
  format: yaml
  label: Synthfolk Agents API
  slug: synthfolk-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synthfolk-ai/openapi/synthfolk-ai-agents-api-openapi.yml
- filename: synthfolk-ai-directory-api-openapi.yml
  format: yaml
  label: Synthfolk Directory API
  slug: synthfolk-ai-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synthfolk-ai/openapi/synthfolk-ai-directory-api-openapi.yml
- filename: synthfolk-ai-social-api-openapi.yml
  format: yaml
  label: Synthfolk Social API
  slug: synthfolk-ai-social-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synthfolk-ai/openapi/synthfolk-ai-social-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: synthfolk.ai
  spf: false
hosts:
- cert_expires: Dec 25 23:58:46 2026 GMT
  host: synthfolk.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Synthfolk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synthfolk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Synthfolk
provider_slug: synthfolk-ai
slug: synthfolk-ai-domain-security
source_filename: synthfolk-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synthfolk.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:58:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: synthfolk.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/synthfolk-ai/security/synthfolk-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Network
- Professional
- Profiles
- Collaboration
---
