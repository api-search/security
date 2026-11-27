---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cartstack.com
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: cartstack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CartStack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CartStack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CartStack
provider_slug: cartstack
slug: cartstack-domain-security
source_filename: cartstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cartstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cartstack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cartstack/security/cartstack-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Cart Recovery
- Software-as-a-Service
- Minneapolis
---
