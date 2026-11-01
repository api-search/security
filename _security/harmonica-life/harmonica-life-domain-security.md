---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: harmonica.life
  spf: false
hosts:
- cert_expires: Jan  7 09:47:47 2027 GMT
  host: harmonica.life
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Harmonica Life Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hawaya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Hawaya
provider_slug: harmonica-life
slug: harmonica-life-domain-security
source_filename: harmonica-life-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: harmonica.life\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 09:47:47 2027 GMT\n  hsts: false\ndomains:\n- domain: harmonica.life\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/harmonica-life/security/harmonica-life-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
