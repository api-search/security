---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: airplatforms.com
  spf: true
hosts:
- cert_expires: Apr 15 00:41:31 2027 GMT
  host: www.airplatforms.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Air Platforms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIR Platforms, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AIR Platforms
provider_slug: air-platforms
slug: air-platforms-domain-security
source_filename: air-platforms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airplatforms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 15 00:41:31 2027 GMT\n  hsts: false\ndomains:\n- domain: airplatforms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/air-platforms/security/air-platforms-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Credit
- Finance
- Risk
---
