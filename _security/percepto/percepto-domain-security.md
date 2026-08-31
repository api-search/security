---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "cloudflare.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: percepto.co
  spf: true
hosts:
- cert_expires: Oct 22 08:18:35 2026 GMT
  host: percepto.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 08:22:53 2026 GMT
  host: drones.percepto.co
  hsts: true
  hsts_max_age: 8640000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Percepto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Percepto, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Percepto
provider_slug: percepto
slug: percepto-domain-security
source_filename: percepto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: percepto.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 08:18:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: drones.percepto.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 08:22:53 2026 GMT\n  hsts: true\n  hsts_max_age: 8640000\ndomains:\n- domain: percepto.co\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"cloudflare.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/percepto/refs/heads/main/security/percepto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Drones
- Robotics
- Industrial Inspection
- Autonomous Systems
- Computer-Vision
- Asset Monitoring
- Energy
- Oil and Gas
- Mining
- Utilities
- Israel
---
