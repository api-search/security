---
api_specs:
- filename: hidemail-app-endpoints-api-openapi.yml
  format: yaml
  label: HideMail Endpoints API
  slug: hidemail-app-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hidemail-app/openapi/hidemail-app-endpoints-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hidemail.app
  spf: true
hosts:
- cert_expires: Jan 24 13:05:04 2027 GMT
  host: hidemail.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HideMail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HideMail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HideMail
provider_slug: hidemail-app
slug: hidemail-app-domain-security
source_filename: hidemail-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hidemail.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 13:05:04 2027 GMT\n  hsts: false\ndomains:\n- domain: hidemail.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hidemail-app/security/hidemail-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Email
- Privacy
- Alias
- Software-as-a-Service
- Free
---
