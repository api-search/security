---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wg-gesucht.de
  spf: true
hosts:
- cert_expires: Dec  3 12:04:22 2026 GMT
  host: wg-gesucht.de
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wg Gesucht Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WG-Gesucht, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WG-Gesucht
provider_slug: wg-gesucht
slug: wg-gesucht-domain-security
source_filename: wg-gesucht-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wg-gesucht.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 12:04:22 2026 GMT\n  hsts: null\ndomains:\n- domain: wg-gesucht.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/wg-gesucht/security/wg-gesucht-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Housing
- Marketplace
- Germany
- Rentals
- SharedFlat
---
