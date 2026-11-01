---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fenris.com
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: fenris.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fenris Creations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fenris Creations, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fenris Creations
provider_slug: fenris-creations
slug: fenris-creations-domain-security
source_filename: fenris-creations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fenris.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: fenris.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fenris-creations/security/fenris-creations-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- VirtualWorlds
- ImmersiveTech
- Gaming
- Platform
---
