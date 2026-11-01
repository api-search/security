---
api_specs:
- filename: dovemails-com-send-api-openapi.yml
  format: yaml
  label: dovemails-com Send API
  slug: dovemails-com-send-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dovemails-com/openapi/dovemails-com-send-api-openapi.yml
- filename: dovemails-com-status-api-openapi.yml
  format: yaml
  label: dovemails-com Status API
  slug: dovemails-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dovemails-com/openapi/dovemails-com-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dovemails.com
  spf: true
hosts:
- cert_expires: Jan 25 17:36:34 2027 GMT
  host: dovemails.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dovemails Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dovemails-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: dovemails-com
provider_slug: dovemails-com
slug: dovemails-com-domain-security
source_filename: dovemails-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dovemails.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 17:36:34 2027 GMT\n  hsts: false\ndomains:\n- domain: dovemails.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dovemails-com/security/dovemails-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Email
- API
- SaaS
- Marketing
---
