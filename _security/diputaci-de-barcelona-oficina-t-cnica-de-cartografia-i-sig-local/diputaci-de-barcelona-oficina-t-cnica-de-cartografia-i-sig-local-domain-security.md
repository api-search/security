---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: diba.cat
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.diba.cat
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Diputaci De Barcelona Oficina T Cnica De Cartografia I Sig Local Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diputació de Barcelona-Oficina Tècnica de Cartografia i Sig Local, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Diputació de Barcelona-Oficina Tècnica de Cartografia i Sig Local
provider_slug: diputaci-de-barcelona-oficina-t-cnica-de-cartografia-i-sig-local
slug: diputaci-de-barcelona-oficina-t-cnica-de-cartografia-i-sig-local-domain-security
source_filename: diputaci-de-barcelona-oficina-t-cnica-de-cartografia-i-sig-local-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.diba.cat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: diba.cat\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/diputaci-de-barcelona-oficina-t-cnica-de-cartografia-i-sig-local/security/diputaci-de-barcelona-oficina-t-cnica-de-cartografia-i-sig-local-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Government
- GIS
- Cartography
- OpenData
---
