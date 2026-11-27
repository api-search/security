---
api_specs:
- filename: talkie-ai-calls-api-openapi.yml
  format: yaml
  label: Talkie.ai Calls API
  slug: talkie-ai-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/talkie-ai/openapi/talkie-ai-calls-api-openapi.yml
- filename: talkie-ai-contacts-api-openapi.yml
  format: yaml
  label: Talkie.ai Contacts API
  slug: talkie-ai-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/talkie-ai/openapi/talkie-ai-contacts-api-openapi.yml
- filename: talkie-ai-data-collection-api-openapi.yml
  format: yaml
  label: Talkie.ai Data Collection API
  slug: talkie-ai-data-collection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/talkie-ai/openapi/talkie-ai-data-collection-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: talkie.ai
  spf: true
hosts:
- cert_expires: Dec 27 18:07:55 2026 GMT
  host: talkie.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Talkie.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Talkie.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Talkie.ai
provider_slug: talkie-ai
slug: talkie-ai-domain-security
source_filename: talkie-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: talkie.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 18:07:55 2026 GMT\n  hsts: false\ndomains:\n- domain: talkie.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/talkie-ai/security/talkie-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Healthcare
- MedicalReceptionist
- HIPAA
---
