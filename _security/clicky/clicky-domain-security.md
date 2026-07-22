---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: clickypass.com
  spf: true
hosts:
- host: clickypass.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Clicky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clicky, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Clicky
provider_slug: clicky
slug: clicky-domain-security
source_filename: clicky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clickypass.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: clickypass.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clicky/refs/heads/main/security/clicky-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Fitness
- Wellness
- Membership
- Subscription
- Marketplace
- Latin America
- Acquired
---
