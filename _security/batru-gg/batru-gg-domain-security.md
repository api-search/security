---
api_specs:
- filename: batru-gg-openapi-generated.yml
  format: yaml
  label: Batru API
  slug: batru-gg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/batru-gg/openapi/_ae-authored/batru-gg-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: batru.gg
  spf: true
hosts:
- cert_expires: Jan 26 07:20:31 2027 GMT
  host: batru.gg
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Batru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Batru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Batru
provider_slug: batru-gg
slug: batru-gg-domain-security
source_filename: batru-gg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: batru.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 07:20:31 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: batru.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/batru-gg/security/batru-gg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gaming
- Esports
- Analytics
- Artificial Intelligence
- Competitive
---
