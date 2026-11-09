---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blumen-verschicken.online
  spf: true
hosts:
- cert_expires: Dec 21 18:38:00 2026 GMT
  host: blumen-verschicken.online
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blumen Verschicken Online Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blumen Komander, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Blumen Komander
provider_slug: blumen-verschicken-online
slug: blumen-verschicken-online-domain-security
source_filename: blumen-verschicken-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blumen-verschicken.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 18:38:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: blumen-verschicken.online\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/blumen-verschicken-online/security/blumen-verschicken-online-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Florist
- E-Commerce
- Germany
- Flowers
---
