---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 4hornind.com
  spf: true
hosts:
- cert_expires: Oct  9 13:23:41 2026 GMT
  host: 4hornind.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 4Hornindustrial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4-Horn Industrial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 4-Horn Industrial
provider_slug: 4hornindustrial
slug: 4hornindustrial-domain-security
source_filename: 4hornindustrial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 4hornind.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:23:41 2026 GMT\n  hsts: false\ndomains:\n- domain: 4hornind.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4hornindustrial/refs/heads/main/security/4hornindustrial-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Equipment Rental
- Industrial Equipment
- Construction
- Energy
- Oil and Gas
- Logistics
- Texas
---
