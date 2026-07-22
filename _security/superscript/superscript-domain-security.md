---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "Sectigo.com"
  - 0 issue "Starfieldtech.com"
  - 0 issue "GoDaddy.com"
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gosuperscript.com
  spf: true
hosts:
- cert_expires: Oct 18 22:47:41 2026 GMT
  host: gosuperscript.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superscript Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superscript, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Superscript
provider_slug: superscript
slug: superscript-domain-security
source_filename: superscript-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gosuperscript.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 22:47:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gosuperscript.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"Sectigo.com\"\n  - 0 issue \"Starfieldtech.com\"\n  - 0 issue \"GoDaddy.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superscript/refs/heads/main/security/superscript-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Business Insurance
- Insurtech
- Cyber Insurance
- Fintech
- United Kingdom
---
