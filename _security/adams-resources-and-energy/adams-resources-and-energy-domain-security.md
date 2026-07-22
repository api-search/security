---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adamsresources.com
  spf: true
hosts:
- cert_expires: Oct  3 06:04:19 2026 GMT
  host: www.adamsresources.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adams Resources And Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adams Resources & Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adams Resources & Energy
provider_slug: adams-resources-and-energy
slug: adams-resources-and-energy-domain-security
source_filename: adams-resources-and-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adamsresources.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:04:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: adamsresources.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adams-resources-and-energy/refs/heads/main/security/adams-resources-and-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Oil And Gas
- Crude Oil
- Transportation
- Logistics
- Midstream
- Petroleum
---
