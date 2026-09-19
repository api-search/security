---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: htktjd.com
  spf: true
hosts:
- host: www.htktjd.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.htktjd.'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aerospacekate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aerospace Kate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aerospace Kate
provider_slug: aerospacekate
slug: aerospacekate-domain-security
source_filename: aerospacekate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  The corporate site is served over plain HTTP. Port 443 does accept a connection, but the\n  certificate presented is a CDN default that does not cover www.htktjd.com (hostname mismatch),\n  so there is no usable HTTPS on the only host this company publishes. No HSTS, no DNSSEC, no\n  CAA and no DMARC record exist for htktjd.com; an SPF record is present. Probed 2026-09-12.\nhosts:\n- host: www.htktjd.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.htktjd.'\n  hsts: null\ndomains:\n- domain: htktjd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerospacekate/refs/heads/main/security/aerospacekate-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Manufacturing
- Robotics
- Industrial Automation
- Motion Control
- Aerospace
- Defense
- Hardware
- China
- No Developer Program
---
