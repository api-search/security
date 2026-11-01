---
api_specs:
- filename: endurain-openapi-generated.yml
  format: yaml
  label: Endurain API
  slug: endurain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/endurain/openapi/_ae-authored/endurain-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: endurain.com
  spf: true
hosts:
- cert_expires: Jan 16 20:15:52 2027 GMT
  host: endurain.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 05:47:37 2027 GMT
  host: docs.endurain.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Endurain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Endurain, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Endurain
provider_slug: endurain
slug: endurain-domain-security
source_filename: endurain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: endurain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 20:15:52 2027 GMT\n  hsts: false\n- host: docs.endurain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 05:47:37 2027 GMT\n  hsts: false\ndomains:\n- domain: endurain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/endurain/security/endurain-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fitness
- Self-hosted
- Open-source
- Privacy
---
