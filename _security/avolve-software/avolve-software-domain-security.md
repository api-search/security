---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: avolvesoftware.com
  spf: true
hosts:
- cert_expires: Feb  7 19:31:25 2027 GMT
  host: avolvesoftware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avolve Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avolve Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Avolve Software
provider_slug: avolve-software
slug: avolve-software-domain-security
source_filename: avolve-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avolvesoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 19:31:25 2027 GMT\n  hsts: false\ndomains:\n- domain: avolvesoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/avolve-software/security/avolve-software-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Software
- Infrastructure
- Government
- GIS
- Plan Review
---
