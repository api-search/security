---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: terragiabiofuel.com
  spf: true
hosts:
- cert_expires: Jan 18 18:44:58 2027 GMT
  host: terragiabiofuel.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Terragiabiofuel Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terragia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Terragia
provider_slug: terragiabiofuel-com
slug: terragiabiofuel-com-domain-security
source_filename: terragiabiofuel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: terragiabiofuel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 18:44:58 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: terragiabiofuel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/terragiabiofuel-com/security/terragiabiofuel-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Biofuels
- Cellulosic Biomass
- Low‑Carbon Fuel
- Transportation Energy
---
