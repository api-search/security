---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gist.ai
  spf: true
hosts:
- cert_expires: Sep 12 01:02:44 2026 GMT
  host: gist.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gist
provider_slug: gist
slug: gist-domain-security
source_filename: gist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gist.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 01:02:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gist.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gist/refs/heads/main/security/gist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Generative AI
- Advertising
- Marketing
- Brand Visibility
- Publishers
- Search
- Content
---
