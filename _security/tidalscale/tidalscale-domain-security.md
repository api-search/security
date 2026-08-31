---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tidalscale.com
  spf: false
hosts:
- host: www.tidalscale.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.tidalsc'
kind: domain-security
layout: security
method: probed
name: Tidalscale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TidalScale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: TidalScale
provider_slug: tidalscale
slug: tidalscale-domain-security
source_filename: tidalscale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tidalscale.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.tidalsc'\n  hsts: null\ndomains:\n- domain: tidalscale.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tidalscale/refs/heads/main/security/tidalscale-domain-security.yml
summary_line: DMARC
tags:
- Company
- Ai Infrastructure
- Server Virtualization
- Software-Defined Infrastructure
- In-Memory Computing
- Acquired
---
