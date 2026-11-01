---
api_specs:
- filename: unifically-com-openapi-generated.yml
  format: yaml
  label: unifically-com API
  slug: unifically-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unifically-com/openapi/_ae-authored/unifically-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unifically.com
  spf: true
hosts:
- cert_expires: Dec 27 13:37:02 2026 GMT
  host: unifically.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Unifically Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for unifically-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: unifically-com
provider_slug: unifically-com
slug: unifically-com-domain-security
source_filename: unifically-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unifically.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 13:37:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: unifically.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/unifically-com/security/unifically-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Media
- Machine-Learning
- Startup
- Platform
---
