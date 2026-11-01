---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: panoramax.fr
  spf: true
hosts:
- cert_expires: Nov 29 05:12:36 2026 GMT
  host: panoramax.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Panoramax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Panoramax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Panoramax
provider_slug: panoramax
slug: panoramax-domain-security
source_filename: panoramax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: panoramax.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 05:12:36 2026 GMT\n  hsts: false\ndomains:\n- domain: panoramax.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/panoramax/security/panoramax-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- OpenData
- Mapping
- Photography
- GIS
---
