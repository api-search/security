---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: graze.social
  spf: false
hosts:
- cert_expires: Jan 10 14:47:43 2027 GMT
  host: graze.social
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Graze Social Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Graze Social, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Graze Social
provider_slug: graze-social
slug: graze-social-domain-security
source_filename: graze-social-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: graze.social\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 14:47:43 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: graze.social\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/graze-social/security/graze-social-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Social
- FeedBuilder
- Bluesky
- API
- SaaS
---
