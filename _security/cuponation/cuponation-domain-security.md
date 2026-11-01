---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: global-savings-group.com
  spf: false
hosts:
- cert_expires: Jan 10 10:05:45 2027 GMT
  host: www.global-savings-group.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cuponation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cuponation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Cuponation
provider_slug: cuponation
slug: cuponation-domain-security
source_filename: cuponation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.global-savings-group.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 10:05:45 2027 GMT\n  hsts: false\ndomains:\n- domain: global-savings-group.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cuponation/security/cuponation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-commerce
- Cashback
- Coupons
- Digital Shopping
---
