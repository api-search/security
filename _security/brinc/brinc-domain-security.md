---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brincdrones.com
  spf: true
hosts:
- cert_expires: Oct 15 01:46:37 2026 GMT
  host: brincdrones.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BRINC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BRINC
provider_slug: brinc
slug: brinc-domain-security
source_filename: brinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brincdrones.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 01:46:37 2026 GMT\n  hsts: false\ndomains:\n- domain: brincdrones.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brinc/refs/heads/main/security/brinc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Drones
- Public Safety
- Law Enforcement
- Emergency Response
- Drone as First Responder
- Hardware
- Software
---
