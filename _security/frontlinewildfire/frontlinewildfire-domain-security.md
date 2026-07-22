---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: frontlinewildfire.com
  spf: true
hosts:
- cert_expires: Sep 30 09:44:15 2026 GMT
  host: frontlinewildfire.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Frontlinewildfire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frontlinewildfire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Frontlinewildfire
provider_slug: frontlinewildfire
slug: frontlinewildfire-domain-security
source_filename: frontlinewildfire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frontlinewildfire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 09:44:15 2026 GMT\n  hsts: false\ndomains:\n- domain: frontlinewildfire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frontlinewildfire/refs/heads/main/security/frontlinewildfire-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Wildfire Defense
- Home Protection
- Fire Safety
- Consumer Hardware
- IoT
- Mobile App
- Sprinkler Systems
- Insurance
---
