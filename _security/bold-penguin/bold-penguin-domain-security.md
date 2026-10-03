---
api_specs:
- filename: bold-penguin-api-openapi-generated.yml
  format: yaml
  label: Bold Penguin api API
  slug: api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-penguin/refs/heads/main/openapi/_ae-authored/bold-penguin-api-openapi-generated.yml
- filename: bold-penguin-core-openapi-generated.yml
  format: yaml
  label: Bold Penguin core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-penguin/refs/heads/main/openapi/_ae-authored/bold-penguin-core-openapi-generated.yml
- filename: bold-penguin-insurance_intelligence-openapi-generated.yml
  format: yaml
  label: Bold Penguin insurance_intelligence API
  slug: insurance_intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bold-penguin/refs/heads/main/openapi/_ae-authored/bold-penguin-insurance_intelligence-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
hosts:
- cert_expires: Dec 18 16:17:45 2026 GMT
  host: forgeglobal.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bold Penguin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bold Penguin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bold Penguin
provider_slug: bold-penguin
slug: bold-penguin-domain-security
source_filename: bold-penguin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 16:17:45 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bold-penguin/refs/heads/main/security/bold-penguin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- API
- Platform
- Commercial
- AI
---
