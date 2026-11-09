---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: briefflink.de
  spf: true
hosts:
- cert_expires: Dec 27 22:47:59 2026 GMT
  host: briefflink.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Briefflink De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Briefflink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Briefflink
provider_slug: briefflink-de
slug: briefflink-de-domain-security
source_filename: briefflink-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: briefflink.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 22:47:59 2026 GMT\n  hsts: false\ndomains:\n- domain: briefflink.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/briefflink-de/security/briefflink-de-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mail
- PDF
- Printing
- Services
---
