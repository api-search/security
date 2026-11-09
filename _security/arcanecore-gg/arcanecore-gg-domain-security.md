---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arcanecore.gg
  spf: true
hosts:
- cert_expires: Jan  2 18:28:36 2027 GMT
  host: arcanecore.gg
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arcanecore Gg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arcane Core, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arcane Core
provider_slug: arcanecore-gg
slug: arcanecore-gg-domain-security
source_filename: arcanecore-gg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arcanecore.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 18:28:36 2027 GMT\n  hsts: false\ndomains:\n- domain: arcanecore.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/arcanecore-gg/security/arcanecore-gg-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- TTRPG
- Live-Display
- Campaign Management
- Gaming
- Web App
---
