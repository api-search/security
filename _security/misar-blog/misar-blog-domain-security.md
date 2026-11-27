---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: misar.blog
  spf: true
hosts:
- cert_expires: Dec 27 17:14:08 2026 GMT
  host: misar.blog
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Misar.Blog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Misar.Blog, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Misar.Blog
provider_slug: misar-blog
slug: misar-blog-domain-security
source_filename: misar-blog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: misar.blog\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 17:14:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: misar.blog\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/misar-blog/security/misar-blog-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blogging
- Artificial Intelligence
- Content Creation
- Platform
- Free
---
