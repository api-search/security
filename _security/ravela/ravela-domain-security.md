---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ravela.com
  spf: true
hosts:
- host: ravela.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: EE certificate key too weak (_ssl.c:1082)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ravela Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ravela Insights, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ravela Insights
provider_slug: ravela
slug: ravela-domain-security
source_filename: ravela-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ravela.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: EE certificate\n    key too weak (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: ravela.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ravela/security/ravela-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Domain
- Parking
- Branding
- Development
---
