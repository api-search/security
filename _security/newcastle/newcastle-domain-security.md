---
api_specs:
- filename: openapi.json
  format: json
  label: Newcastle Urban Observatory API
  slug: urban-observatory
  spec_type: OpenAPI
  url: https://api.usb.urbanobservatory.ac.uk/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ncl.ac.uk
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: urbanobservatory.ac.uk
  spf: false
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: www.ncl.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 15 02:02:59 2026 GMT
  host: api.usb.urbanobservatory.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  9 12:50:32 2026 GMT
  host: api-dor.ncl.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Newcastle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Newcastle University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Newcastle University
provider_slug: newcastle
slug: newcastle-domain-security
source_filename: newcastle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ncl.ac.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.usb.urbanobservatory.ac.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 15 02:02:59 2026 GMT\n  hsts: false\n- host: api-dor.ncl.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 12:50:32 2026 GMT\n  hsts: false\ndomains:\n- domain: ncl.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: urbanobservatory.ac.uk\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/security/newcastle-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- United Kingdom
- Open Data
- Research Data
- Smart Cities
- Digital Library
---
