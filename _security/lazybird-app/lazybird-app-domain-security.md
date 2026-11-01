---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lazybird.app
  spf: true
hosts:
- cert_expires: Dec 18 05:43:05 2026 GMT
  host: lazybird.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 20:27:10 2026 GMT
  host: www.lazybird.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 05:10:50 2027 GMT
  host: api.lazybird.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Lazybird App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lazybird-app, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: lazybird-app
provider_slug: lazybird-app
slug: lazybird-app-domain-security
source_filename: lazybird-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lazybird.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 05:43:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.lazybird.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 20:27:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.lazybird.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 05:10:50 2027 GMT\n  hsts: false\ndomains:\n- domain: lazybird.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lazybird-app/security/lazybird-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Voiceover
- Text-to-Speech
- Creator Tools
- Multilingual
---
