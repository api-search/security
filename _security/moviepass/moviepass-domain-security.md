---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: moviepass.com
  spf: true
hosts:
- cert_expires: Aug 29 05:09:24 2026 GMT
  host: www.moviepass.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moviepass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moviepass, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Moviepass
provider_slug: moviepass
slug: moviepass-domain-security
source_filename: moviepass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moviepass.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 05:09:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: moviepass.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moviepass/refs/heads/main/security/moviepass-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Movies
- Entertainment
- Subscription
- Consumer
- Streaming and Media
- Ticketing
---
