---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 iodef "mailto:caa-alerts@hopper.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hopper.com
  spf: true
hosts:
- cert_expires: Aug 24 06:23:20 2026 GMT
  host: hopper.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 16:34:25 2026 GMT
  host: hts.hopper.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hopper Travel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hopper, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Hopper
provider_slug: hopper-travel
slug: hopper-travel-domain-security
source_filename: hopper-travel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hopper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 06:23:20 2026 GMT\n  hsts: null\n- host: hts.hopper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 16:34:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hopper.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 iodef \"mailto:caa-alerts@hopper.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopper-travel/refs/heads/main/security/hopper-travel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Travel
- Marketplace
- Fintech
- Price Freeze
- Insurance
- B2B
- Embedded
- Agentic AI
- Banks
- Airlines
---
