---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: astonsci.com
  spf: true
hosts:
- host: astonsci.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''astonsci.co'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Astonsci Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astonsci, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Astonsci
provider_slug: astonsci
slug: astonsci-domain-security
source_filename: astonsci-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: astonsci.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''astonsci.co'\n  hsts: null\ndomains:\n- domain: astonsci.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astonsci/refs/heads/main/security/astonsci-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Biopharma
- Clinical-stage
- Innovation
- Medicine
- SouthKorea
---
