---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Pixelfed REST API
  slug: pixelfed-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pixelfed.org
  spf: true
hosts:
- cert_expires: Sep  9 10:17:04 2026 GMT
  host: docs.pixelfed.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pixelfed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pixelfed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pixelfed
provider_slug: pixelfed
slug: pixelfed-domain-security
source_filename: pixelfed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.pixelfed.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 10:17:04 2026 GMT\n  hsts: false\ndomains:\n- domain: pixelfed.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/security/pixelfed-domain-security.yml
summary_line: TLSv1.3
tags:
- Fediverse
- ActivityPub
- Photo Sharing
- Social Media
- Open Source
- Decentralized
- Mastodon Compatible
- Federation
---
