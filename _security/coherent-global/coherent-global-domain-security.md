---
api_specs:
- filename: coherent-global-openapi-generated.yml
  format: yaml
  label: Coherent API
  slug: coherent-global-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coherent-global/openapi/_ae-authored/coherent-global-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: coherent.global
  spf: true
hosts:
- cert_expires: Feb 10 08:07:20 2027 GMT
  host: coherent.global
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coherent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coherent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Coherent
provider_slug: coherent-global
slug: coherent-global-domain-security
source_filename: coherent-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coherent.global\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 08:07:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coherent.global\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/coherent-global/security/coherent-global-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Excel
- Automation
- Insurance
- Finance
---
