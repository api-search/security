---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: suwayomi.org
  spf: true
hosts:
- cert_expires: Jan 16 09:50:18 2027 GMT
  host: suwayomi.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Suwayomi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Suwayomi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Suwayomi
provider_slug: suwayomi
slug: suwayomi-domain-security
source_filename: suwayomi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: suwayomi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 09:50:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: suwayomi.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/suwayomi/security/suwayomi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Manga
- OpenSource
- Media
- Server
- Community
---
