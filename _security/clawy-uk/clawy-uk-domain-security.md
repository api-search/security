---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clawy.uk
  spf: true
hosts:
- cert_expires: Jan 10 19:13:46 2027 GMT
  host: clawy.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clawy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clawy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clawy
provider_slug: clawy-uk
slug: clawy-uk-domain-security
source_filename: clawy-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clawy.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 19:13:46 2027 GMT\n  hsts: false\ndomains:\n- domain: clawy.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/clawy-uk/security/clawy-uk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Automation
- Node
- Beta
- Control
---
