---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elcheff.com.mx
  spf: true
hosts:
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: elcheff.com.mx
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: El Cheff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for El Cheff, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: El Cheff
provider_slug: elcheff-com-mx
slug: elcheff-com-mx-domain-security
source_filename: elcheff-com-mx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elcheff.com.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: elcheff.com.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/elcheff-com-mx/security/elcheff-com-mx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Point-of-Sale
- Restaurant
- Software
- Mexico
- Software-as-a-Service
---
