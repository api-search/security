---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: numbersstation.ai
  mx: google-workspace
  spf: false
hosts:
- host: numbersstation.ai
  hsts: null
  hsts_max_age: null
  https: false
  tls_error: ERR_SSL_VERSION_OR_CIPHER_MISMATCH
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Numbersstation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Numbersstation, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Numbersstation
provider_slug: numbersstation
slug: numbersstation-domain-security
source_filename: numbersstation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: dig + TLS handshake probe (numbersstation.ai)\nnote: >-\n  The apex host numbersstation.ai (WP Engine, 141.193.213.10/11) currently\n  refuses the TLS handshake for every client probed (system curl/LibreSSL,\n  Python urllib, headless Chromium via reader proxy) with\n  ERR_SSL_VERSION_OR_CIPHER_MISMATCH, so HTTPS reachability/HSTS/cert could\n  not be captured. DNS-level records were probed directly with dig.\nhosts:\n  - host: numbersstation.ai\n    https: false\n    tls_version: null\n    tls_error: ERR_SSL_VERSION_OR_CIPHER_MISMATCH\n    hsts: null\n    hsts_max_age: null\ndomains:\n  - domain: numbersstation.ai\n    dnssec: false\n    caa: []\n    spf: false\n    dmarc: false\n    dmarc_policy: null\n    mx: google-workspace\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numbersstation/refs/heads/main/security/numbersstation-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Unknown
---
