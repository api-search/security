---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: letitrain.com
  spf: true
hosts:
- host: letitrain.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Letitrain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Rainmaker Group Ventures (letitrain.com), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Rainmaker Group Ventures (letitrain.com)
provider_slug: letitrain
slug: letitrain-domain-security
source_filename: letitrain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: letitrain.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: letitrain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/letitrain/refs/heads/main/security/letitrain-domain-security.yml
summary_line: DMARC
tags:
- Company
- Hospitality
- Revenue Management
- Hotels
- Casinos
- Business Intelligence
- Pricing
- Defunct
---
