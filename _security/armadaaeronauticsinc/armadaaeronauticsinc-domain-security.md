---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: armadaaero.com
  spf: true
hosts:
- host: armadaaero.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''armadaaero.'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Armadaaeronauticsinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Armadaaeronauticsinc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Armadaaeronauticsinc
provider_slug: armadaaeronauticsinc
slug: armadaaeronauticsinc-domain-security
source_filename: armadaaeronauticsinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: armadaaero.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''armadaaero.'\n  hsts: null\ndomains:\n- domain: armadaaero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armadaaeronauticsinc/refs/heads/main/security/armadaaeronauticsinc-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Mobility
- Transportation
- Urban
- Innovation
---
