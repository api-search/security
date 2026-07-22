---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: true
  domain: news-corporation.com
  spf: false
hosts:
- host: www.news-corporation.com
  https: false
kind: domain-security
layout: security
method: probed
name: News Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for news-corporation, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: news-corporation
provider_slug: news-corporation
slug: news-corporation-domain-security
source_filename: news-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.news-corporation.com\n  https: false\ndomains:\n- domain: news-corporation.com\n  dnssec: true\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/news-corporation/refs/heads/main/security/news-corporation-domain-security.yml
summary_line: DNSSEC
tags:
- Fortune 500
---
