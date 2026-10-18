---
api_specs:
- filename: infere-openapi-generated.yml
  format: yaml
  label: Snowball Studio Ltd. API
  slug: infere-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infere/refs/heads/main/openapi/_ae-authored/infere-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: infere.com
  spf: true
hosts:
- cert_expires: Dec 23 13:33:45 2026 GMT
  host: infere.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Infere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snowball Studio Ltd., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Snowball Studio Ltd.
provider_slug: infere
slug: infere-domain-security
source_filename: infere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 13:33:45 2026 GMT\n  hsts: false\ndomains:\n- domain: infere.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infere/refs/heads/main/security/infere-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Observability
- PromptManagement
- LLM
---
