---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cma-cgm.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cma-cgm.net
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.cma-cgm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: api-portal.cma-cgm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: apis.cma-cgm.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cma Cgm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CMA CGM, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CMA CGM
provider_slug: cma-cgm
slug: cma-cgm-domain-security
source_filename: cma-cgm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cma-cgm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: null\n- host: api-portal.cma-cgm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apis.cma-cgm.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cma-cgm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cma-cgm.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cma-cgm/refs/heads/main/security/cma-cgm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Shipping
- Container Shipping
- Maritime
- Logistics
- Freight
- Supply Chain
- Ports
- Terminals
- Track and Trace
- DCSA
- EDI
- Air Cargo
- Intermodal
- Ocean Freight
- Smart Containers
---
