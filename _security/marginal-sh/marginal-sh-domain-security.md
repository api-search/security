---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: marginal.sh
  spf: false
hosts:
- cert_expires: Jan  4 00:57:16 2027 GMT
  host: marginal.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Prime Broker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prime Broker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Prime Broker
provider_slug: marginal-sh
slug: marginal-sh-domain-security
source_filename: marginal-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marginal.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 00:57:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: marginal.sh\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/marginal-sh/security/marginal-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
