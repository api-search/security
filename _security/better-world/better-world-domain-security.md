---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: betterworldbooks.com
  spf: true
hosts:
- cert_expires: Dec  1 15:36:04 2026 GMT
  host: www.betterworldbooks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Better World Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Better World Books, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Better World Books
provider_slug: better-world
slug: better-world-domain-security
source_filename: better-world-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.betterworldbooks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 15:36:04 2026 GMT\n  hsts: null\ndomains:\n- domain: betterworldbooks.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/better-world/refs/heads/main/security/better-world-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Books
- Retail
- Literacy
- E-commerce
---
