---
api_specs:
- filename: e2a-dev-api-openapi.yml
  format: yaml
  label: e2a API API
  slug: e2a-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/e2a-dev/openapi/_original/e2a-dev-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: e2a.dev
  spf: true
hosts:
- cert_expires: Dec 15 05:56:04 2026 GMT
  host: e2a.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: E2A Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for e2a-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: e2a-dev
provider_slug: e2a-dev
slug: e2a-dev-domain-security
source_filename: e2a-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: e2a.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 05:56:04 2026 GMT\n  hsts: false\ndomains:\n- domain: e2a.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/e2a-dev/security/e2a-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Email
- OpenSource
- API
- AI
---
