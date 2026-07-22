---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: aerodome.com
  spf: true
hosts:
- cert_expires: Sep 16 22:03:45 2026 GMT
  host: www.aerodome.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aerodome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aerodome, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Aerodome
provider_slug: aerodome
slug: aerodome-domain-security
source_filename: aerodome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aerodome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 22:03:45 2026 GMT\n  hsts: false\ndomains:\n- domain: aerodome.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerodome/refs/heads/main/security/aerodome-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Drones
- Drone as First Responder
- Public Safety
- Law Enforcement
- Emergency Response
- Defense Tech
- Aerial Intelligence
- Autonomous Systems
---
