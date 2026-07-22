---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:domains@eero.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eero.com
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: eero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Eero
provider_slug: eero
slug: eero-domain-security
source_filename: eero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: eero.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:domains@eero.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eero/refs/heads/main/security/eero-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Networking
- WiFi
- Mesh Networking
- Home Networking
- Smart Home
- Internet of Things
- Hardware
- Consumer Electronics
---
