---
api_specs:
- filename: chorilo-com-openapi-generated.yml
  format: yaml
  label: Chorilo API
  slug: chorilo-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chorilo-com/openapi/_ae-authored/chorilo-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chorilo.com
  spf: true
hosts:
- cert_expires: Dec 12 02:56:00 2026 GMT
  host: chorilo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chorilo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chorilo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chorilo
provider_slug: chorilo-com
slug: chorilo-com-domain-security
source_filename: chorilo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chorilo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 02:56:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chorilo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/chorilo-com/security/chorilo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Choir Management
- Sheet Music
- Event Planning
- Finance
- Membership
- Collaboration
- GDPR
- Mobile App
---
