---
api_specs:
- filename: lemmebuyit-com-changes-api-openapi.yml
  format: yaml
  label: LemMeBuyIt Changes API
  slug: lemmebuyit-com-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lemmebuyit-com/openapi/lemmebuyit-com-changes-api-openapi.yml
- filename: lemmebuyit-com-promotions-api-openapi.yml
  format: yaml
  label: LemMeBuyIt Promotions API
  slug: lemmebuyit-com-promotions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lemmebuyit-com/openapi/lemmebuyit-com-promotions-api-openapi.yml
- filename: lemmebuyit-com-retailers-api-openapi.yml
  format: yaml
  label: LemMeBuyIt Retailers API
  slug: lemmebuyit-com-retailers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lemmebuyit-com/openapi/lemmebuyit-com-retailers-api-openapi.yml
- filename: lemmebuyit-com-status-api-openapi.yml
  format: yaml
  label: LemMeBuyIt Status API
  slug: lemmebuyit-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lemmebuyit-com/openapi/lemmebuyit-com-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lemmebuyit.com
  spf: true
hosts:
- cert_expires: Jan  2 20:06:47 2027 GMT
  host: lemmebuyit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LemMeBuyIt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LemMeBuyIt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LemMeBuyIt
provider_slug: lemmebuyit-com
slug: lemmebuyit-com-domain-security
source_filename: lemmebuyit-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lemmebuyit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 20:06:47 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lemmebuyit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lemmebuyit-com/security/lemmebuyit-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Retail
- Real-Time Data
- Product Intelligence
- AI Agents
---
