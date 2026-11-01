---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: westfalenwind.de
  spf: true
hosts:
- cert_expires: Jan 20 19:53:08 2027 GMT
  host: westfalenwind.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Westfalenwind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WestfalenWIND, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WestfalenWIND
provider_slug: westfalenwind
slug: westfalenwind-domain-security
source_filename: westfalenwind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: westfalenwind.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 19:53:08 2027 GMT\n  hsts: false\ndomains:\n- domain: westfalenwind.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/westfalenwind/security/westfalenwind-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Renewable Energy
- Wind Power
- Germany
- Sustainable
---
