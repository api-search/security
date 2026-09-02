---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nekosia.cat
  spf: true
hosts:
- cert_expires: Nov  6 05:45:01 2026 GMT
  host: nekosia.cat
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 05:45:01 2026 GMT
  host: api.nekosia.cat
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nekosia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nekosia API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Nekosia API
provider_slug: nekosia
slug: nekosia-domain-security
source_filename: nekosia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nekosia.cat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 05:45:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nekosia.cat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 05:45:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nekosia.cat\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nekosia/refs/heads/main/security/nekosia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Anime
- neko
- nekos
- neko api
- booru
- Image
- Media
- Entertainment
- Free API
- Open Access
---
