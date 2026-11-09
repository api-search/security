---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: asha.news
  spf: true
hosts:
- cert_expires: Dec 26 09:35:26 2026 GMT
  host: asha.news
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asha News Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asha News, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Asha News
provider_slug: asha-news
slug: asha-news-domain-security
source_filename: asha-news-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asha.news\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 09:35:26 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: asha.news\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/asha-news/security/asha-news-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- News
- Evidence-first
- Conflict
- Palestine
- Journalism
---
