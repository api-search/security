---
api_specs:
- filename: getinboxzero-com-rules-api-openapi.yml
  format: yaml
  label: Inbox Zero Rules API
  slug: getinboxzero-com-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getinboxzero-com/openapi/getinboxzero-com-rules-api-openapi.yml
- filename: getinboxzero-com-senders-api-openapi.yml
  format: yaml
  label: Inbox Zero Senders API
  slug: getinboxzero-com-senders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getinboxzero-com/openapi/getinboxzero-com-senders-api-openapi.yml
- filename: getinboxzero-com-stats-api-openapi.yml
  format: yaml
  label: Inbox Zero Stats API
  slug: getinboxzero-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getinboxzero-com/openapi/getinboxzero-com-stats-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getinboxzero.com
  spf: true
hosts:
- cert_expires: Jan 30 18:41:00 2027 GMT
  host: getinboxzero.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Inbox Zero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inbox Zero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Inbox Zero
provider_slug: getinboxzero-com
slug: getinboxzero-com-domain-security
source_filename: getinboxzero-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getinboxzero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 18:41:00 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getinboxzero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/getinboxzero-com/security/getinboxzero-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Management
- AI Assistant
- Email Automation
- Open Source
---
