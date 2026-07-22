---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chemix.ai
  spf: true
hosts:
- cert_expires: Sep 25 17:48:17 2026 GMT
  host: www.chemix.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chemix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chemix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Chemix
provider_slug: chemix
slug: chemix-domain-security
source_filename: chemix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chemix.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:48:17 2026 GMT\n  hsts: false\ndomains:\n- domain: chemix.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chemix/refs/heads/main/security/chemix-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Battery
- Energy
- Power Systems
- Observability
- Electric Vehicles
- Deep Tech
---
