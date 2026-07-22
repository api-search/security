---
api_specs:
- filename: nationbuilder-v2-openapi-original.yml
  format: yaml
  label: NationBuilder v2 API
  slug: nationbuilder-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nationbuilder/refs/heads/main/openapi/nationbuilder-v2-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nationbuilder.com
  spf: true
hosts:
- cert_expires: Sep 29 13:20:06 2026 GMT
  host: nationbuilder.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nationbuilder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NationBuilder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NationBuilder
provider_slug: nationbuilder
slug: nationbuilder-domain-security
source_filename: nationbuilder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nationbuilder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:20:06 2026 GMT\n  hsts: null\ndomains:\n- domain: nationbuilder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nationbuilder/refs/heads/main/security/nationbuilder-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Community Organizing
- CRM
- Political
- Nonprofit
- Fundraising
- Advocacy
- Website Builder
- Events
- Email
- JSON:API
---
