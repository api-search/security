---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: landmarkglobal.com
  spf: true
hosts:
- cert_expires: Jan  6 06:05:57 2027 GMT
  host: landmarkglobal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Landmark Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Landmark Global, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Landmark Global
provider_slug: landmark-global
slug: landmark-global-domain-security
source_filename: landmark-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: landmarkglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 06:05:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: landmarkglobal.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/landmark-global/security/landmark-global-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- E-commerce
- Shipping
- API
---
