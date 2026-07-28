---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: neso.energy
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: carbonintensity.org.uk
  spf: false
hosts:
- cert_expires: Aug 30 15:27:23 2026 GMT
  host: www.neso.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 17:07:34 2026 GMT
  host: api.neso.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: api.carbonintensity.org.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Energy System Operator (NESO), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Energy System Operator (NESO)
provider_slug: neso
slug: neso-domain-security
source_filename: neso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neso.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 15:27:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.neso.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 17:07:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.carbonintensity.org.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: neso.energy\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: carbonintensity.org.uk\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neso/refs/heads/main/security/neso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- United Kingdom
- Electricity
- Energy Markets
- Grid
- Open Data
- Carbon
- Renewables
- Gas
- Demand Response
---
