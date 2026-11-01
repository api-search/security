---
api_specs:
- filename: olaclick-openapi-generated.yml
  format: yaml
  label: OlaClick API
  slug: olaclick-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/olaclick/openapi/_ae-authored/olaclick-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: olaclick.com
  spf: true
hosts:
- cert_expires: Dec  2 12:45:16 2026 GMT
  host: www.olaclick.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Olaclick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OlaClick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OlaClick
provider_slug: olaclick
slug: olaclick-domain-security
source_filename: olaclick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.olaclick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 12:45:16 2026 GMT\n  hsts: false\ndomains:\n- domain: olaclick.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/olaclick/security/olaclick-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Restaurant
- POS
- AI
- SaaS
- Delivery
---
