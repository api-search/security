---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "geotrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anydesk.com
  spf: true
hosts:
- cert_expires: Oct 13 11:28:13 2026 GMT
  host: anydesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anydesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AnyDesk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AnyDesk
provider_slug: anydesk
slug: anydesk-domain-security
source_filename: anydesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anydesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 11:28:13 2026 GMT\n  hsts: null\ndomains:\n- domain: anydesk.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"geotrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anydesk/refs/heads/main/security/anydesk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Remote Work
- Remote Desktop
- Remote Access
- Remote Support
- IT Management
- REST API
- Security
---
