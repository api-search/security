---
api_specs:
- filename: princeton-allsearch-api-openapi.yml
  format: yaml
  label: Princeton University Library Allsearch API
  slug: allsearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-allsearch-api-openapi.yml
- filename: princeton-art-museum-api-openapi.yml
  format: yaml
  label: Princeton University Art Museum API
  slug: art-museum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/openapi/princeton-art-museum-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: princeton.edu
  spf: true
hosts:
- cert_expires: Aug 30 00:57:27 2026 GMT
  host: www.princeton.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 23:59:59 2026 GMT
  host: data.artmuseum.princeton.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api-store.princeton.edu
  https: false
kind: domain-security
layout: security
method: probed
name: Princeton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Princeton University, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Princeton University
provider_slug: princeton
slug: princeton-domain-security
source_filename: princeton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.princeton.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 00:57:27 2026 GMT\n  hsts: false\n- host: data.artmuseum.princeton.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:59:59 2026 GMT\n  hsts: null\n- host: api-store.princeton.edu\n  https: false\ndomains:\n- domain: princeton.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/princeton/refs/heads/main/security/princeton-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- University
- Higher Education
- Education
- Ivy League
- United States
- New Jersey
- Research Library
- Research Data
- Open Data
- Digital Collections
- Identity Federation
- Museum
---
