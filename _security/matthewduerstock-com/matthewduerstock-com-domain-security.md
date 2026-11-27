---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: matthewduerstock.com
  spf: true
hosts:
- cert_expires: Feb  8 20:33:47 2027 GMT
  host: matthewduerstock.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: matthewduerstock-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for matthewduerstock-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: matthewduerstock-com
provider_slug: matthewduerstock-com
slug: matthewduerstock-com-domain-security
source_filename: matthewduerstock-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: matthewduerstock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 20:33:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: matthewduerstock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/matthewduerstock-com/security/matthewduerstock-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
