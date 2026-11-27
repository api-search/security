---
api_specs:
- filename: regiai-com-openapi-generated.yml
  format: yaml
  label: RegiAI API
  slug: regiai-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regiai-com/openapi/_ae-authored/regiai-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: true
  domain: regiai.com
  spf: false
hosts:
- cert_expires: Jan 29 07:13:09 2027 GMT
  host: regiai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: RegiAI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RegiAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: RegiAI
provider_slug: regiai-com
slug: regiai-com-domain-security
source_filename: regiai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: regiai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 07:13:09 2027 GMT\n  hsts: false\ndomains:\n- domain: regiai.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/regiai-com/security/regiai-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- AI
- Video
- Image
- Audio
- Platform
---
