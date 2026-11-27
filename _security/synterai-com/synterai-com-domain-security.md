---
api_specs:
- filename: synterai-com-openapi-generated.yml
  format: yaml
  label: Synter API
  slug: synterai-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synterai-com/openapi/_ae-authored/synterai-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: synterai.com
  spf: true
hosts:
- cert_expires: Feb  2 23:59:06 2027 GMT
  host: synterai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Synter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Synter
provider_slug: synterai-com
slug: synterai-com-domain-security
source_filename: synterai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synterai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:06 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: synterai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/synterai-com/security/synterai-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- AI
- Marketing
- Automation
- Platform
---
