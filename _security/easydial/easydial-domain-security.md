---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: easydial.io
  spf: true
hosts:
- cert_expires: Nov 24 20:50:08 2026 GMT
  host: www.easydial.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Easydial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Easydial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Easydial
provider_slug: easydial
slug: easydial-domain-security
source_filename: easydial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.easydial.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 20:50:08 2026 GMT\n  hsts: false\ndomains:\n- domain: easydial.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/easydial/security/easydial-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Communications
- AI
- Unified-Communications
- Contact-Center
---
