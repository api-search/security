---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: upteamco.com
  spf: true
hosts:
- cert_expires: Aug 19 23:02:34 2026 GMT
  host: upteamco.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upteam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upteam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Upteam
provider_slug: upteam
slug: upteam-domain-security
source_filename: upteam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upteamco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:02:34 2026 GMT\n  hsts: false\ndomains:\n- domain: upteamco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upteam/refs/heads/main/security/upteam-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Luxury Resale
- B2B
- Pre-owned Goods
- Portfolio Company
---
