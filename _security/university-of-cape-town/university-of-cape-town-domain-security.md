---
api_specs:
- filename: university-of-cape-town-datafirst-nada.yaml
  format: yaml
  label: DataFirst Microdata Catalog API (NADA)
  slug: datafirst-nada
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-cape-town/refs/heads/main/openapi/university-of-cape-town-datafirst-nada.yaml
description: ''
domains:
- caa:
  - 0 issue "harica.gr"
  - 0 issuewild "harica.gr"
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uct.ac.za
  spf: true
hosts:
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: www.uct.ac.za
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: www.datafirst.uct.ac.za
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  9 11:30:25 2027 GMT
  host: open.uct.ac.za
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Cape Town Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Cape Town, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: University of Cape Town
provider_slug: university-of-cape-town
slug: university-of-cape-town-domain-security
source_filename: university-of-cape-town-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uct.ac.za\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: null\n- host: www.datafirst.uct.ac.za\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\n- host: open.uct.ac.za\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 11:30:25 2027 GMT\n  hsts: false\ndomains:\n- domain: uct.ac.za\n  dnssec: true\n  caa:\n  - 0 issue \"harica.gr\"\n  - 0 issuewild \"harica.gr\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-cape-town/refs/heads/main/security/university-of-cape-town-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Data
- Institutional Repository
- OAI-PMH
- South Africa
- Africa
---
