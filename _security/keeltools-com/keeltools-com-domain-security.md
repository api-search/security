---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: keeltools.com
  spf: true
hosts:
- cert_expires: Jan  9 03:33:42 2027 GMT
  host: keeltools.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KeelTools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KeelTools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: KeelTools
provider_slug: keeltools-com
slug: keeltools-com-domain-security
source_filename: keeltools-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keeltools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 03:33:42 2027 GMT\n  hsts: false\ndomains:\n- domain: keeltools.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/keeltools-com/security/keeltools-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Tools
- Directory
- Coding
- Productivity
- Creative
- Business
- Research
- Entertainment
---
