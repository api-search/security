---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ottodata.app
  spf: false
hosts:
- cert_expires: Feb 10 03:32:47 2027 GMT
  host: ottodata.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Otto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Otto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Otto
provider_slug: ottodata-app
slug: ottodata-app-domain-security
source_filename: ottodata-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ottodata.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 03:32:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ottodata.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ottodata-app/security/ottodata-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Cryptocurrency
- Data
- Market Intelligence
- Onchain
---
