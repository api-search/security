---
api_specs:
- filename: freeq-at-openapi.yml
  format: yaml
  label: freeq IRC API
  slug: freeq-irc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeq-at/openapi/freeq-at-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freeq.at
  spf: true
hosts:
- cert_expires: Jan 30 17:34:06 2027 GMT
  host: freeq.at
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: freeq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for freeq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: freeq
provider_slug: freeq-at
slug: freeq-at-domain-security
source_filename: freeq-at-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freeq.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 17:34:06 2027 GMT\n  hsts: false\ndomains:\n- domain: freeq.at\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/freeq-at/security/freeq-at-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Chat
- Identity
- Encryption
- Open Source
- Irc
---
