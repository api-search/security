---
api_specs:
- filename: mailkite-dev-openapi-generated.yml
  format: yaml
  label: mailkite-dev API
  slug: mailkite-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailkite-dev/openapi/_ae-authored/mailkite-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mailkite.dev
  spf: true
hosts:
- cert_expires: Jan 23 15:13:12 2027 GMT
  host: mailkite.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mailkite Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mailkite-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: mailkite-dev
provider_slug: mailkite-dev
slug: mailkite-dev-domain-security
source_filename: mailkite-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailkite.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 15:13:12 2027 GMT\n  hsts: false\ndomains:\n- domain: mailkite.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mailkite-dev/security/mailkite-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Email
- API
- SaaS
- Communication
---
