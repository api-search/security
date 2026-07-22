---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tallylabs.co
  spf: true
hosts:
- host: tallylabs.co
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''tallylabs.c'
kind: domain-security
layout: security
method: probed
name: Tally Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tally Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tally Labs
provider_slug: tally-labs
slug: tally-labs-domain-security
source_filename: tally-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tallylabs.co\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''tallylabs.c'\n  hsts: null\ndomains:\n- domain: tallylabs.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tally-labs/refs/heads/main/security/tally-labs-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Web3
- NFT
- Media
- Entertainment
- Blockchain
- Storytelling
---
