---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deutschepost.de
  spf: true
hosts:
- cert_expires: Dec 26 08:00:06 2026 GMT
  host: deutschepost.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deutsche Post Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deutsche Post, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Deutsche Post
provider_slug: deutsche-post
slug: deutsche-post-domain-security
source_filename: deutsche-post-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deutschepost.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 08:00:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: deutschepost.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/deutsche-post/security/deutsche-post-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Postal
- Logistics
- Shipping
- E‑commerce
---
