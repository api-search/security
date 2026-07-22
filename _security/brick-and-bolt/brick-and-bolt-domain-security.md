---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bricknbolt.com
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: www.bricknbolt.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Brick And Bolt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brick&Bolt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brick&Bolt
provider_slug: brick-and-bolt
slug: brick-and-bolt-domain-security
source_filename: brick-and-bolt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bricknbolt.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: bricknbolt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brick-and-bolt/refs/heads/main/security/brick-and-bolt-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Marketplaces
- Construction
- Home Building
- Real Estate
- Proptech
- India
- Project Management
---
