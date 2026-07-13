---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: penguinrandomhouse.biz
  spf: false
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: www.penguinrandomhouse.biz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Penguin Publishing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Penguin Publishing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Penguin Publishing
provider_slug: penguin-publishing
slug: penguin-publishing-domain-security
source_filename: penguin-publishing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.penguinrandomhouse.biz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: penguinrandomhouse.biz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/penguin-publishing/refs/heads/main/security/penguin-publishing-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Books
- Public APIs
---
