---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: waystationai.com
  spf: true
hosts:
- cert_expires: Apr  6 23:59:59 2027 GMT
  host: waystationai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Waystation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Waystation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Waystation
provider_slug: waystation
slug: waystation-domain-security
source_filename: waystation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: waystationai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: waystationai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/waystation/security/waystation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Sourcing
- CPG
- Procurement
---
