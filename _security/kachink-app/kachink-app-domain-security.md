---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kachink.app
  spf: true
hosts:
- cert_expires: Jan 20 06:27:39 2027 GMT
  host: kachink.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kachink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kachink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kachink
provider_slug: kachink-app
slug: kachink-app-domain-security
source_filename: kachink-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kachink.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 06:27:39 2027 GMT\n  hsts: false\ndomains:\n- domain: kachink.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kachink-app/security/kachink-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Finance
- Artificial Intelligence
- Personal Finance
- Multi-Currency
- Software-as-a-Service
---
