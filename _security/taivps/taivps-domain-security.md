---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: taivps.net
  spf: true
hosts:
- cert_expires: Dec 18 09:19:55 2026 GMT
  host: taivps.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Taivps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TaiVPS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TaiVPS
provider_slug: taivps
slug: taivps-domain-security
source_filename: taivps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taivps.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 09:19:55 2026 GMT\n  hsts: false\ndomains:\n- domain: taivps.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taivps/refs/heads/main/security/taivps-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud VPS
- Web Hosting
- Reseller Hosting
- Domains
- Infrastructure
- Vietnam
---
