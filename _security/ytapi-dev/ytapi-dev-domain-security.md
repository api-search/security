---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ytapi.dev
  spf: true
hosts:
- cert_expires: Dec 18 02:06:59 2026 GMT
  host: ytapi.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ytapi-dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ytapi-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ytapi-dev
provider_slug: ytapi-dev
slug: ytapi-dev-domain-security
source_filename: ytapi-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ytapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 02:06:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ytapi.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ytapi-dev/security/ytapi-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Video
- Transcripts
- YouTube
---
