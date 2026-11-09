---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bitacora.live
  spf: true
hosts:
- cert_expires: Dec 20 22:26:24 2026 GMT
  host: bitacora.live
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bitacora Live Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitácora, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bitácora
provider_slug: bitacora-live
slug: bitacora-live-domain-security
source_filename: bitacora-live-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitacora.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 22:26:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: bitacora.live\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bitacora-live/security/bitacora-live-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Design
- Collaboration
- UI/UX
- Software-as-a-Service
- Free Tier
---
