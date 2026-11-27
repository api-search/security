---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: buzzfy.co
  spf: true
hosts:
- cert_expires: Dec 25 14:23:30 2026 GMT
  host: buzzfy.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buzzfy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buzzfy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Buzzfy
provider_slug: buzzfy-co
slug: buzzfy-co-domain-security
source_filename: buzzfy-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buzzfy.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 14:23:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buzzfy.co\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/buzzfy-co/security/buzzfy-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Instagram
- Growth
- Analytics
- Social Media
---
