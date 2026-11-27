---
api_specs:
- filename: connic-co-public-openapi.json
  format: json
  label: connic API Public API
  slug: connic-api-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/connic-co/openapi/_original/connic-co-public-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: connic.co
  spf: true
hosts:
- cert_expires: Dec 31 23:51:09 2026 GMT
  host: connic.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Connic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Connic
provider_slug: connic-co
slug: connic-co-domain-security
source_filename: connic-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: connic.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:51:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: connic.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/connic-co/security/connic-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Platform
- Munich
- Automation
---
