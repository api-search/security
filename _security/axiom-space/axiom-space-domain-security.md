---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: axiomspace.com
  spf: true
hosts:
- cert_expires: Oct 16 14:57:46 2026 GMT
  host: www.axiomspace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axiom Space Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axiom Space, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Axiom Space
provider_slug: axiom-space
slug: axiom-space-domain-security
source_filename: axiom-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.axiomspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 14:57:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: axiomspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axiom-space/refs/heads/main/security/axiom-space-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Aerospace
- Space
- Commercial Spaceflight
- Space Station
- Human Spaceflight
- Microgravity Research
- In-Space Manufacturing
- Spacesuits
- Orbital Data Center
- Edge Computing
- Government Contractor
---
