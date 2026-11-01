---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: justflip.com
  spf: true
hosts:
- host: justflip.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''justflip.co'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Justflip Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Flip
provider_slug: justflip-com
slug: justflip-com-domain-security
source_filename: justflip-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justflip.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''justflip.co'\n  hsts: null\ndomains:\n- domain: justflip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/justflip-com/security/justflip-com-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Startup
- VC-backed
- Lightspeed-Venture-Partners
- Y-Combinator
---
