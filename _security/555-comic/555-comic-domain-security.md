---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 555comic.com
  spf: true
hosts:
- cert_expires: Sep 27 17:00:19 2026 GMT
  host: 555comic.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 555 Comic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 555 Comic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 555 Comic
provider_slug: 555-comic
slug: 555-comic-domain-security
source_filename: 555-comic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 555comic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:00:19 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: 555comic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/555-comic/refs/heads/main/security/555-comic-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Entertainment
- Media
- Storytelling
- Virtual Influencers
- Anime
- Social Media
- ARG
---
