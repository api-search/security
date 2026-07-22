---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anheuser-busch.com
  spf: true
hosts:
- cert_expires: Sep 24 05:29:14 2026 GMT
  host: www.anheuser-busch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anheuser Busch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anheuser-Busch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Anheuser-Busch
provider_slug: anheuser-busch
slug: anheuser-busch-domain-security
source_filename: anheuser-busch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anheuser-busch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 05:29:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anheuser-busch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anheuser-busch/refs/heads/main/security/anheuser-busch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Beverages
- Consumer Goods
- Manufacturing
---
