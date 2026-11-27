---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getrefine.co
  spf: true
hosts:
- cert_expires: Jan  5 06:19:32 2027 GMT
  host: getrefine.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Refine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Refine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Refine
provider_slug: getrefine-co
slug: getrefine-co-domain-security
source_filename: getrefine-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getrefine.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 06:19:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getrefine.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/getrefine-co/security/getrefine-co-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Job Search
- Professional Networking
- Careers
- Recruiting
- Platform
---
