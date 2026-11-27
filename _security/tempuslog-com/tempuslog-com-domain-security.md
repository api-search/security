---
api_specs:
- filename: tempuslog-com-openapi-generated.yml
  format: yaml
  label: TempusLog API
  slug: tempuslog-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tempuslog-com/openapi/_ae-authored/tempuslog-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tempuslog.com
  spf: false
hosts:
- cert_expires: Dec 29 15:35:53 2026 GMT
  host: tempuslog.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TempusLog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TempusLog, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: TempusLog
provider_slug: tempuslog-com
slug: tempuslog-com-domain-security
source_filename: tempuslog-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tempuslog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 15:35:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tempuslog.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tempuslog-com/security/tempuslog-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Time Tracking
- SaaS
- Free
- EU Data
- Team Collaboration
---
