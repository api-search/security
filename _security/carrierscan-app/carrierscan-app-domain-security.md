---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: carrierscan.app
  spf: false
hosts:
- cert_expires: Jan 13 17:06:36 2027 GMT
  host: carrierscan.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: carrierscan-app Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for carrierscan-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: carrierscan-app
provider_slug: carrierscan-app
slug: carrierscan-app-domain-security
source_filename: carrierscan-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carrierscan.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 17:06:36 2027 GMT\n  hsts: false\ndomains:\n- domain: carrierscan.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/carrierscan-app/security/carrierscan-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
