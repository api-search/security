---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: orbismedicines.com
  spf: true
hosts:
- cert_expires: Nov 22 11:58:58 2026 GMT
  host: www.orbismedicines.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Orbis Medicines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orbis Medicines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Orbis Medicines
provider_slug: orbis-medicines
slug: orbis-medicines-domain-security
source_filename: orbis-medicines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.orbismedicines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 11:58:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: orbismedicines.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/orbis-medicines/security/orbis-medicines-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotech
- AI
- Drug Discovery
- Oral Therapeutics
---
