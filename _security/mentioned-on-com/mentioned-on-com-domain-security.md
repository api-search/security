---
api_specs:
- filename: mentioned-on-com-openapi-generated.yml
  format: yaml
  label: MentionedOn API
  slug: mentioned-on-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mentioned-on-com/openapi/_ae-authored/mentioned-on-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mentioned-on.com
  spf: true
hosts:
- cert_expires: Jan  6 21:46:29 2027 GMT
  host: mentioned-on.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MentionedOn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MentionedOn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: MentionedOn
provider_slug: mentioned-on-com
slug: mentioned-on-com-domain-security
source_filename: mentioned-on-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mentioned-on.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 21:46:29 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mentioned-on.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mentioned-on-com/security/mentioned-on-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Visibility
- Local Business
- Monitoring
- Services
---
