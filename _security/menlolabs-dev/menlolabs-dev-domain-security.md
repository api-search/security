---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: menlolabs.dev
  spf: true
hosts:
- cert_expires: Feb 11 08:52:14 2027 GMT
  host: menlolabs.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: menlolabs-dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for menlolabs-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: menlolabs-dev
provider_slug: menlolabs-dev
slug: menlolabs-dev-domain-security
source_filename: menlolabs-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: menlolabs.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 08:52:14 2027 GMT\n  hsts: null\ndomains:\n- domain: menlolabs.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/menlolabs-dev/security/menlolabs-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
