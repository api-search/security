---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kaufliste.ch
  spf: false
hosts:
- cert_expires: Dec 27 15:11:47 2026 GMT
  host: kaufliste.ch
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kaufliste.ch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaufliste.ch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Kaufliste.ch
provider_slug: kaufliste-ch
slug: kaufliste-ch-domain-security
source_filename: kaufliste-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kaufliste.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 15:11:47 2026 GMT\n  hsts: false\ndomains:\n- domain: kaufliste.ch\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kaufliste-ch/security/kaufliste-ch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Shopping
- Grocery
- List
- Swiss
- Family
---
