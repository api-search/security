---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: gameshopenter.com
  spf: true
hosts:
- cert_expires: Dec 11 15:53:51 2026 GMT
  host: gameshopenter.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gameshop Enter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gameshop Enter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Gameshop Enter
provider_slug: gameshopenter-com
slug: gameshopenter-com-domain-security
source_filename: gameshopenter-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gameshopenter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 15:53:51 2026 GMT\n  hsts: null\ndomains:\n- domain: gameshopenter.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gameshopenter-com/security/gameshopenter-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Retail
- Video Games
- Retro Gaming
- Dutch Business
- E-Commerce
---
