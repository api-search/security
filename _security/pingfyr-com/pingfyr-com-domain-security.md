---
api_specs:
- filename: pingfyr-com-openapi-generated.yml
  format: yaml
  label: pingfyr-com API
  slug: pingfyr-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pingfyr-com/openapi/_ae-authored/pingfyr-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pingfyr.com
  spf: false
hosts:
- cert_expires: Jan 19 11:20:16 2027 GMT
  host: pingfyr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pingfyr Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pingfyr-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: pingfyr-com
provider_slug: pingfyr-com
slug: pingfyr-com-domain-security
source_filename: pingfyr-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pingfyr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 11:20:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pingfyr.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/pingfyr-com/security/pingfyr-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- API
- Scheduling
- Notifications
- Webhooks
- AI
---
