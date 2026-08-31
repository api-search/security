---
api_specs:
- filename: newcastle-digitised-objects-api-openapi.yml
  format: yaml
  label: Digitised Objects Repository Search and Data API
  slug: digitised-objects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-digitised-objects-api-openapi.yml
- filename: newcastle-entity-api-openapi.yml
  format: yaml
  label: Urban Observatory API (Urban Sciences Building) — Entity
  slug: urban-observatory-entity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-entity-api-openapi.yml
- filename: newcastle-feed-api-openapi.yml
  format: yaml
  label: Urban Observatory API (Urban Sciences Building) — Feed
  slug: urban-observatory-feed
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-feed-api-openapi.yml
- filename: newcastle-summary-api-openapi.yml
  format: yaml
  label: Urban Observatory API (Urban Sciences Building) — Summary
  slug: urban-observatory-summary
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-summary-api-openapi.yml
- filename: newcastle-timeseries-api-openapi.yml
  format: yaml
  label: Urban Observatory API (Urban Sciences Building) — Timeseries
  slug: urban-observatory-timeseries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-timeseries-api-openapi.yml
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
method: derived
name: Newcastle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Newcastle University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Newcastle University
provider_slug: newcastle
slug: newcastle-domain-security
source_filename: newcastle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nx-evidence-method: probed\nx-provenance-note: >-\n  Written by API Evangelist's probe-domain-security.py from live DNS and TLS observations\n  of Newcastle University hosts. Not a Newcastle-published document.\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ncl.ac.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.usb.urbanobservatory.ac.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 15 02:02:59 2026 GMT\n  hsts: false\n- host: api-dor.ncl.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 12:50:32 2026 GMT\n  hsts: false\ndomains:\n- domain: ncl.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: urbanobservatory.ac.uk\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/security/newcastle-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- United Kingdom
- Russell Group
- Research Data
- Open Data
- Digital Library
- Identity Federation
- Smart Cities
- Cultural Heritage
---
