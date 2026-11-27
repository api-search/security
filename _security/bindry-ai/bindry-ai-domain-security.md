---
api_specs:
- filename: bindry-ai-openapi-generated.yml
  format: yaml
  label: Bindry API
  slug: bindry-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bindry-ai/openapi/_ae-authored/bindry-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bindry.ai
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: bindry.ai
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bindry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bindry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bindry
provider_slug: bindry-ai
slug: bindry-ai-domain-security
source_filename: bindry-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bindry.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: bindry.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bindry-ai/security/bindry-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Package Manager
- Skills
- Developer Tools
- Open Source
- Company
---
