---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: maktapp.com
  spf: false
hosts:
- cert_expires: Dec 24 04:39:12 2026 GMT
  host: maktapp.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Maktapp Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fatora, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Fatora
provider_slug: maktapp-com
slug: maktapp-com-domain-security
source_filename: maktapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maktapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 04:39:12 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: maktapp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/maktapp-com/security/maktapp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
