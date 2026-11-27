---
api_specs:
- filename: flow2-co-openapi-generated.yml
  format: yaml
  label: Flow2 API
  slug: flow2-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flow2-co/openapi/_ae-authored/flow2-co-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flow2.co
  spf: true
hosts:
- cert_expires: Jan 30 20:08:06 2027 GMT
  host: flow2.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flow2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flow2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Flow2
provider_slug: flow2-co
slug: flow2-co-domain-security
source_filename: flow2-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flow2.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 20:08:06 2027 GMT\n  hsts: false\ndomains:\n- domain: flow2.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/flow2-co/security/flow2-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Presentation
- Mobile
- Interactive
- FlowVella
---
