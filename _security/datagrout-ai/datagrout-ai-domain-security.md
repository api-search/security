---
api_specs:
- filename: datagrout-ai-openapi-generated.yml
  format: yaml
  label: DataGrout API
  slug: datagrout-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datagrout-ai/openapi/_ae-authored/datagrout-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: datagrout.ai
  spf: true
hosts:
- cert_expires: Jan  2 09:28:54 2027 GMT
  host: datagrout.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datagrout Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataGrout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DataGrout
provider_slug: datagrout-ai
slug: datagrout-ai-domain-security
source_filename: datagrout-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datagrout.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 09:28:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: datagrout.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/datagrout-ai/security/datagrout-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Enterprise
- Platform
- Memory
- Tools
---
