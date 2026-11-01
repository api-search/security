---
api_specs:
- filename: enable-com-openapi-generated.yml
  format: yaml
  label: Enable API
  slug: enable-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enable-com/openapi/_ae-authored/enable-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: enable.com
  spf: true
hosts:
- cert_expires: Jan 22 22:58:16 2027 GMT
  host: enable.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Enable Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Enable
provider_slug: enable-com
slug: enable-com-domain-security
source_filename: enable-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: enable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 22:58:16 2027 GMT\n  hsts: false\ndomains:\n- domain: enable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/enable-com/security/enable-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Pricing
- Rebate
- SaaS
- AI
- Pricing
- Rebate
- SaaS
---
