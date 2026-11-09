---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apricot.tools
  spf: false
hosts:
- cert_expires: Jan  3 11:46:46 2027 GMT
  host: apricot.tools
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apricot Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for apricot-tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: apricot-tools
provider_slug: apricot-tools
slug: apricot-tools-domain-security
source_filename: apricot-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apricot.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 11:46:46 2027 GMT\n  hsts: false\ndomains:\n- domain: apricot.tools\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/apricot-tools/security/apricot-tools-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
