---
api_specs:
- filename: ottic-plants-api-openapi.yml
  format: yaml
  label: Ottic API
  slug: ottic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ottic/openapi/ottic-plants-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ottic.ai
  spf: false
hosts:
- cert_expires: Dec  1 02:06:51 2026 GMT
  host: ottic.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ottic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ottic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Ottic
provider_slug: ottic
slug: ottic-domain-security
source_filename: ottic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ottic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 02:06:51 2026 GMT\n  hsts: false\ndomains:\n- domain: ottic.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ottic/security/ottic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Automation
- Productivity
- Agents
- Platform
---
