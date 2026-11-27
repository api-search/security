---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: connectmyshop.app
  spf: true
hosts:
- cert_expires: Jan 17 21:08:31 2027 GMT
  host: connectmyshop.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ConnectMyShop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConnectMyShop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ConnectMyShop
provider_slug: connectmyshop-app
slug: connectmyshop-app-domain-security
source_filename: connectmyshop-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: connectmyshop.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 21:08:31 2027 GMT\n  hsts: false\ndomains:\n- domain: connectmyshop.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/connectmyshop-app/security/connectmyshop-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Etsy
- E-Commerce
- AI Assistant
- MCP
- Shop Management
- Discontinued
---
