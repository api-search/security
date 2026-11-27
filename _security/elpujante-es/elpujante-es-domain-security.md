---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: elpujante.es
  spf: true
hosts:
- cert_expires: Dec 22 02:45:15 2026 GMT
  host: elpujante.es
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: El Pujante Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for El Pujante, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: El Pujante
provider_slug: elpujante-es
slug: elpujante-es-domain-security
source_filename: elpujante-es-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elpujante.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 02:45:15 2026 GMT\n  hsts: false\ndomains:\n- domain: elpujante.es\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/elpujante-es/security/elpujante-es-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real Estate
- Auctions
- Artificial Intelligence
- Spain
- Platform
---
