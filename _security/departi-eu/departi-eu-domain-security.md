---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: departi.eu
  spf: true
hosts:
- cert_expires: Dec 13 19:28:55 2026 GMT
  host: departi.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Departi Eu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Departi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Departi
provider_slug: departi-eu
slug: departi-eu-domain-security
source_filename: departi-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: departi.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 19:28:55 2026 GMT\n  hsts: false\ndomains:\n- domain: departi.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/departi-eu/security/departi-eu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Digital Nomads
- Accommodation
- Visa
- MCP
- AI Concierge
- Europe
---
