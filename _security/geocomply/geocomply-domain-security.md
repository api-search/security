---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: geocomply.com
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: geocomply.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geocomply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geocomply, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Geocomply
provider_slug: geocomply
slug: geocomply-domain-security
source_filename: geocomply-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geocomply.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: geocomply.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geocomply/refs/heads/main/security/geocomply-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Geolocation
- Compliance
- Fraud Prevention
- Identity Verification
- KYC
- Anti-Fraud
- iGaming
- Financial Services
- Security
---
