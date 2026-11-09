---
api_specs:
- filename: domduck-com-openapi-generated.yml
  format: yaml
  label: Domduck API
  slug: domduck-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domduck-com/openapi/_ae-authored/domduck-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: domduck.com
  spf: true
hosts:
- cert_expires: Dec 29 15:05:12 2026 GMT
  host: domduck.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Domduck Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Domduck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Domduck
provider_slug: domduck-com
slug: domduck-com-domain-security
source_filename: domduck-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domduck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 15:05:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: domduck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/domduck-com/security/domduck-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Domain Reputation
- Monitoring
- Free Tier
- Dashboards
---
