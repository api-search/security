---
api_specs:
- filename: dscout-openapi-generated.yml
  format: yaml
  label: dscout API
  slug: dscout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dscout/openapi/_ae-authored/dscout-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dscout.com
  spf: true
hosts:
- cert_expires: Jan 17 09:13:16 2027 GMT
  host: dscout.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dscout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dscout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: dscout
provider_slug: dscout
slug: dscout-domain-security
source_filename: dscout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dscout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 09:13:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dscout.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dscout/security/dscout-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- UX Research
- AI
- User Testing
- Market Research
---
