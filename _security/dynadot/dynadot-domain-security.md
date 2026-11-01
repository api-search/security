---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dynadot.com
  spf: true
hosts:
- cert_expires: Dec  4 23:16:51 2026 GMT
  host: dynadot.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dynadot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dynadot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dynadot
provider_slug: dynadot
slug: dynadot-domain-security
source_filename: dynadot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dynadot.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:16:51 2026 GMT\n  hsts: false\ndomains:\n- domain: dynadot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dynadot/security/dynadot-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Domain Registrar
- Marketplace
- DNS Management
- SSL
---
