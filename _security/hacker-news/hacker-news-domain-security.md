---
api_specs:
- filename: hacker-news-openapi.yml
  format: yaml
  label: Hacker News API
  slug: hacker-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacker-news/refs/heads/main/openapi/hacker-news-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ycombinator.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: firebaseio.com
  spf: true
hosts:
- cert_expires: Aug 15 08:05:33 2026 GMT
  host: news.ycombinator.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 15:01:46 2026 GMT
  host: hacker-news.firebaseio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hacker News Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hacker News, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hacker News
provider_slug: hacker-news
slug: hacker-news-domain-security
source_filename: hacker-news-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: news.ycombinator.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 08:05:33 2026 GMT\n  hsts: null\n- host: hacker-news.firebaseio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:01:46 2026 GMT\n  hsts: null\ndomains:\n- domain: ycombinator.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: firebaseio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hacker-news/refs/heads/main/security/hacker-news-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Developer Community
- Technology News
- Y Combinator
---
