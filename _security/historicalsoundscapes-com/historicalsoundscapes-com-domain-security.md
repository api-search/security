---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: historicalsoundscapes.com
  spf: true
hosts:
- cert_expires: Dec 22 08:20:17 2026 GMT
  host: historicalsoundscapes.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Historical Soundscapes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Historical Soundscapes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Historical Soundscapes
provider_slug: historicalsoundscapes-com
slug: historicalsoundscapes-com-domain-security
source_filename: historicalsoundscapes-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: historicalsoundscapes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 08:20:17 2026 GMT\n  hsts: false\ndomains:\n- domain: historicalsoundscapes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/historicalsoundscapes-com/security/historicalsoundscapes-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
