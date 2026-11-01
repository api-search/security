---
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: fyyd.de
  spf: true
hosts:
- cert_expires: Jan 13 15:45:16 2027 GMT
  host: fyyd.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fyyd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fyyd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: fyyd
provider_slug: fyyd
slug: fyyd-domain-security
source_filename: fyyd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fyyd.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 15:45:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fyyd.de\n  dnssec: false\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fyyd/security/fyyd-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Podcast
- Search
- Directory
- Audio
- Germany
- Company
---
