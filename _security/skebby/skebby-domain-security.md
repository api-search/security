---
api_specs:
- filename: skebby-openapi-generated.yml
  format: yaml
  label: Skebby API
  slug: skebby-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skebby/openapi/_ae-authored/skebby-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: skebby.it
  spf: true
hosts:
- cert_expires: Apr  7 23:59:59 2027 GMT
  host: skebby.it
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Skebby Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skebby, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Skebby
provider_slug: skebby
slug: skebby-domain-security
source_filename: skebby-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skebby.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: skebby.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/skebby/security/skebby-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SMS
- Messaging
- Italy
- Marketing
---
