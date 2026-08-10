---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: autofleet.io
  spf: true
hosts:
- cert_expires: Oct 14 23:44:35 2026 GMT
  host: autofleet.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 05:06:05 2026 GMT
  host: api.autofleet.io
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autofleet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autofleet, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Autofleet
provider_slug: autofleet
slug: autofleet-domain-security
source_filename: autofleet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: autofleet.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:44:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.autofleet.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 05:06:05 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: autofleet.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nnotes:\n- >-\n  api.autofleet.io sends a Strict-Transport-Security header with max-age=0,\n  which explicitly DISABLES HSTS for the API host rather than enforcing it. The\n  header is present but inert. The marketing host autofleet.io sets a real\n  max-age=31536000. Recorded as observed.\n- >-\n  api.autofleet.io otherwise ships a strong default header set (helmet-style):\n  Content-Security-Policy default-src 'self', Cross-Origin-Embedder-Policy\n  require-corp, Cross-Origin-Opener-Policy\
  \ same-origin,\n  Cross-Origin-Resource-Policy same-origin, Referrer-Policy no-referrer,\n  X-Content-Type-Options nosniff, X-Frame-Options SAMEORIGIN. Both hosts sit\n  behind Cloudflare.\n- >-\n  No CAA records and no DNSSEC on autofleet.io. SPF and DMARC are both present;\n  the DMARC policy is p=quarantine.\n- >-\n  No vulnerability-disclosure program and no trust center were found:\n  /.well-known/security.txt is 404 on every host, and trust.autofleet.io,\n  security.autofleet.io and status.autofleet.io do not resolve. probe-security-\n  programs.py reported vdp=none trust=none, so no VulnerabilityDisclosure,\n  Security or TrustCenter artifact or pointer is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autofleet/refs/heads/main/security/autofleet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fleet Management
- Mobility
- Transportation
- Logistics
- Route Optimization
- Dispatch
- Last Mile Delivery
- Car Sharing
- Telematics
- Artificial Intelligence
---
