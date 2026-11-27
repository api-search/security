---
api_specs:
- filename: lorglabs-com-api-openapi.json
  format: json
  label: Lorg Check Api API
  slug: lorg-check-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lorglabs-com/openapi/_original/lorglabs-com-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lorglabs.com
  spf: true
hosts:
- cert_expires: Jan 12 14:57:46 2027 GMT
  host: lorglabs.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lorg Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lorg Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Lorg Labs
provider_slug: lorglabs-com
slug: lorglabs-com-domain-security
source_filename: lorglabs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lorglabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 14:57:46 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: lorglabs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lorglabs-com/security/lorglabs-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Safety
- Risk Assessment
- Automation
- Artificial Intelligence
---
