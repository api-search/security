---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mywine.dev
  spf: true
hosts:
- cert_expires: Jan 29 08:52:18 2027 GMT
  host: mywine.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: My Wine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for My Wine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: My Wine
provider_slug: mywine-dev
slug: mywine-dev-domain-security
source_filename: mywine-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mywine.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 08:52:18 2027 GMT\n  hsts: false\ndomains:\n- domain: mywine.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mywine-dev/security/mywine-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Wine
- Marketplace
- Data
- Transparency
- Shopping
---
