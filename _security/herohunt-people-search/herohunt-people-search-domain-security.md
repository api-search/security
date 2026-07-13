---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: herohunt.ai
  spf: true
hosts:
- cert_expires: Aug 20 09:49:53 2026 GMT
  host: www.herohunt.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Herohunt People Search Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HeroHunt People Search, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HeroHunt People Search
provider_slug: herohunt-people-search
slug: herohunt-people-search-domain-security
source_filename: herohunt-people-search-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.herohunt.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 09:49:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: herohunt.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/herohunt-people-search/refs/heads/main/security/herohunt-people-search-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Jobs
- Public APIs
---
