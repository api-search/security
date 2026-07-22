---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 451degrees.com
  spf: true
hosts:
- host: www.451degrees.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: 451 Degrees Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 451 Degrees, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 451 Degrees
provider_slug: 451-degrees
slug: 451-degrees-domain-security
source_filename: 451-degrees-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.451degrees.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: 451degrees.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/451-degrees/refs/heads/main/security/451-degrees-domain-security.yml
summary_line: DMARC
tags:
- Company
- Artificial Intelligence
- Ad Tech
- Brand Safety
- Contextual Advertising
- Content Moderation
- Natural Language Processing
- Machine Learning
- Marketing Technology
- Privacy
---
