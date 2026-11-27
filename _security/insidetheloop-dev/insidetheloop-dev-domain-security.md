---
api_specs:
- filename: insidetheloop-dev-openapi-generated.yml
  format: yaml
  label: Inside the Loop API
  slug: insidetheloop-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insidetheloop-dev/openapi/_ae-authored/insidetheloop-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: insidetheloop.dev
  spf: true
hosts:
- cert_expires: Dec 27 23:11:24 2026 GMT
  host: insidetheloop.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Inside the Loop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inside the Loop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Inside the Loop
provider_slug: insidetheloop-dev
slug: insidetheloop-dev-domain-security
source_filename: insidetheloop-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insidetheloop.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:11:24 2026 GMT\n  hsts: false\ndomains:\n- domain: insidetheloop.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/insidetheloop-dev/security/insidetheloop-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Tools
- Fixes
- Guides
- Agents
- Developer Tools
---
