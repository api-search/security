---
api_specs:
- filename: opsive-openapi-generated.yml
  format: yaml
  label: Opsive API
  slug: opsive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opsive/openapi/_ae-authored/opsive-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opsive.com
  spf: true
hosts:
- cert_expires: Nov 30 07:34:45 2026 GMT
  host: opsive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Opsive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opsive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Opsive
provider_slug: opsive
slug: opsive-domain-security
source_filename: opsive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opsive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 07:34:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opsive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/opsive/security/opsive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Game Development
- Unity
- Artificial Intelligence
- Behavior Trees
- Character Controllers
- Inventory Systems
- Developer Tools
---
