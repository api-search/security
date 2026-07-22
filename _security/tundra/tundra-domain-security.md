---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: tundra.com
  spf: true
hosts:
- host: www.tundra.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Tundra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tundra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Tundra
provider_slug: tundra
slug: tundra-domain-security
source_filename: tundra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tundra.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: tundra.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tundra/refs/heads/main/security/tundra-domain-security.yml
summary_line: DNSSEC
tags:
- Company
- Ecommerce
- Marketplace
- Wholesale
- Retail
- B2B
---
