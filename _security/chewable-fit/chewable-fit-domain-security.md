---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chewable.app
  spf: false
hosts:
- cert_expires: Dec 30 17:33:47 2026 GMT
  host: chewable.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chewable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chewable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Chewable
provider_slug: chewable-fit
slug: chewable-fit-domain-security
source_filename: chewable-fit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chewable.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 17:33:47 2026 GMT\n  hsts: false\ndomains:\n- domain: chewable.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/chewable-fit/security/chewable-fit-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Mobile App
- iOS
- Recipes
- Meal Planning
- Fitness
- Strength Training
- Fashion
- Virtual Try-On
- Artificial Intelligence
- MCP
---
