---
api_specs:
- filename: brandyze-fr-openapi-generated.yml
  format: yaml
  label: Brandyze API
  slug: brandyze-fr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brandyze-fr/openapi/_ae-authored/brandyze-fr-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brandyze.fr
  spf: true
hosts:
- cert_expires: Dec 26 12:42:19 2026 GMT
  host: brandyze.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brandyze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brandyze, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Brandyze
provider_slug: brandyze-fr
slug: brandyze-fr-domain-security
source_filename: brandyze-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brandyze.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 12:42:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brandyze.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/brandyze-fr/security/brandyze-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Marketing
- Content Generation
- Brand Analysis
- Creator Tools
---
