---
api_specs:
- filename: aeon-fun-api-openapi.json
  format: json
  label: aeon agent-facing API API
  slug: aeon-agent-facing-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aeon-fun/openapi/_original/aeon-fun-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aeon.fun
  spf: false
hosts:
- cert_expires: Dec 20 23:54:59 2026 GMT
  host: aeon.fun
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aeon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aeon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Aeon
provider_slug: aeon-fun
slug: aeon-fun-domain-security
source_filename: aeon-fun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aeon.fun\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:54:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aeon.fun\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aeon-fun/security/aeon-fun-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Automation
- Open Source
- Framework
- Enterprise
---
