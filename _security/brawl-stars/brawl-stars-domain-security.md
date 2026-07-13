---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brawlstars.com
  spf: false
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: developer.brawlstars.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brawl Stars Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brawl Stars, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Brawl Stars
provider_slug: brawl-stars
slug: brawl-stars-domain-security
source_filename: brawl-stars-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.brawlstars.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: brawlstars.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brawl-stars/refs/heads/main/security/brawl-stars-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---
