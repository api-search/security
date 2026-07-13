---
api_specs:
- filename: llms.txt
  format: yaml
  label: SignWell API
  slug: signwell-api
  spec_type: OpenAPI
  url: https://developers.signwell.com/llms.txt
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: signwell.com
  spf: true
hosts:
- cert_expires: Oct  3 11:44:26 2026 GMT
  host: www.signwell.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 19:59:21 2026 GMT
  host: developers.signwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Signwell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SignWell, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SignWell
provider_slug: signwell
slug: signwell-domain-security
source_filename: signwell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.signwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 11:44:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.signwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 19:59:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: signwell.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signwell/refs/heads/main/security/signwell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Signature
- Electronic Signature
- Documents
- PDF
- Signing
- Templates
- Workflows
- HIPAA
- SOC2
---
