---
api_specs:
- filename: vikunja-openapi-generated.yml
  format: yaml
  label: Vikunja API
  slug: vikunja-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vikunja/openapi/_ae-authored/vikunja-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vikunja.io
  spf: true
hosts:
- cert_expires: Dec 26 16:43:49 2026 GMT
  host: vikunja.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vikunja Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vikunja, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Vikunja
provider_slug: vikunja
slug: vikunja-domain-security
source_filename: vikunja-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vikunja.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 16:43:49 2026 GMT\n  hsts: false\ndomains:\n- domain: vikunja.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/vikunja/security/vikunja-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- OpenSource
- TaskManagement
- SelfHostable
- European
---
