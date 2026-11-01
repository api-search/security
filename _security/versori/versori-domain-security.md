---
api_specs:
- filename: versori-platform-openapi.yml
  format: yaml
  label: Versori Platform API
  slug: versori-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/versori/openapi/versori-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: versori.com
  spf: true
hosts:
- cert_expires: Jan  9 06:53:20 2027 GMT
  host: versori.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Versori Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Versori, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Versori
provider_slug: versori
slug: versori-domain-security
source_filename: versori-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: versori.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 06:53:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: versori.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/versori/security/versori-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Integration
- Artificial Intelligence
- Automation
- Platform
---
