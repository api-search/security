---
api_specs:
- filename: usertapes-com-openapi-generated.yml
  format: yaml
  label: UserTapes API
  slug: usertapes-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usertapes-com/openapi/_ae-authored/usertapes-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: usertapes.com
  spf: true
hosts:
- cert_expires: Feb 17 20:59:36 2027 GMT
  host: usertapes.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: UserTapes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UserTapes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: UserTapes
provider_slug: usertapes-com
slug: usertapes-com-domain-security
source_filename: usertapes-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usertapes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 20:59:36 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: usertapes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/usertapes-com/security/usertapes-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Session Replay
- AI Integration
- Analytics
- Privacy
- Monitoring
---
