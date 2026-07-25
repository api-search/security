---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ensurance.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chaseunderwriting.com.au
  spf: true
hosts:
- host: ensurance.com.au
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
- cert_expires: Sep 11 22:34:13 2026 GMT
  host: www.chaseunderwriting.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: 3rdp.ensurance.com.au
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Ensurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ensurance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ensurance
provider_slug: ensurance
slug: ensurance-domain-security
source_filename: ensurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ensurance.com.au\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\n- host: www.chaseunderwriting.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 22:34:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: 3rdp.ensurance.com.au\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: ensurance.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: chaseunderwriting.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ensurance/refs/heads/main/security/ensurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Australia
- Underwriting
- Property and Casualty
- Construction Insurance
- Managing General Agent
- Broker
- Wholesale Insurance
- Insurtech
- Partner Gated
- No Public API
---
