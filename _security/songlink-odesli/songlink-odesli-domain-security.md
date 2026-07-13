---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: notion.so
  spf: true
hosts:
- cert_expires: Sep 13 23:41:14 2026 GMT
  host: www.notion.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Songlink Odesli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Songlink / Odesli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Songlink / Odesli
provider_slug: songlink-odesli
slug: songlink-odesli-domain-security
source_filename: songlink-odesli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.notion.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:41:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: notion.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/songlink-odesli/refs/heads/main/security/songlink-odesli-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Public APIs
---
