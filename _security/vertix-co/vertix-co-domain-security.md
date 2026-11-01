---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vertix.co
  spf: true
hosts:
- cert_expires: Dec 28 05:52:54 2026 GMT
  host: vertix.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vertix Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VeriTX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VeriTX
provider_slug: vertix-co
slug: vertix-co-domain-security
source_filename: vertix-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vertix.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 05:52:54 2026 GMT\n  hsts: false\ndomains:\n- domain: vertix.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/vertix-co/security/vertix-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Materials
- Foundry
- Machinery
- Supply-Chain
- Metallurgy
---
