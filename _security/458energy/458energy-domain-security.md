---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 458energy.com
  spf: true
hosts:
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: 458energy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 458Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 45-8 ENERGY, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 45-8 ENERGY
provider_slug: 458energy
slug: 458energy-domain-security
source_filename: 458energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 458energy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: 458energy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/458energy/refs/heads/main/security/458energy-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Energy
- Helium
- Natural Hydrogen
- Natural Resources
- Exploration and Production
- Industrial Gases
- Cleantech
- France
---
