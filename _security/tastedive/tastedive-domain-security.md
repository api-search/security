---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tastedive.com
  spf: true
hosts:
- cert_expires: Sep 11 22:48:28 2026 GMT
  host: tastedive.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tastedive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TasteDive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TasteDive
provider_slug: tastedive
slug: tastedive-domain-security
source_filename: tastedive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tastedive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 22:48:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tastedive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tastedive/refs/heads/main/security/tastedive-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Entertainment
- Public APIs
---
