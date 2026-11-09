---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: a1.gallery
  spf: true
hosts:
- cert_expires: Dec  4 00:49:52 2026 GMT
  host: a1.gallery
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: A1 Gallery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for A1 Gallery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: A1 Gallery
provider_slug: a1-gallery
slug: a1-gallery-domain-security
source_filename: a1-gallery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: a1.gallery\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 00:49:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: a1.gallery\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/a1-gallery/security/a1-gallery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Design
- Gallery
- Web
- Creative
---
