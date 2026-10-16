---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bookmyhost.com
  spf: true
hosts:
- cert_expires: Jan  6 11:32:59 2027 GMT
  host: bookmyhost.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bookmyhost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blazing Bullet Private Limited, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blazing Bullet Private Limited
provider_slug: bookmyhost
slug: bookmyhost-domain-security
source_filename: bookmyhost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bookmyhost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 11:32:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: bookmyhost.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bookmyhost/refs/heads/main/security/bookmyhost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud
- Hosting
- VPS
- India
---
