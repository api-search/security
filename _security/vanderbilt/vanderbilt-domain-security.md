---
api_specs:
- filename: vanderbilt-television-news-archive-openapi.yml
  format: yaml
  label: Vanderbilt Television News Archive API
  slug: television-news-archive
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanderbilt/refs/heads/main/openapi/vanderbilt-television-news-archive-openapi.yml
- filename: vanderbilt-sparql-openapi.yml
  format: yaml
  label: Vanderbilt Libraries SPARQL Endpoint
  slug: sparql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanderbilt/refs/heads/main/openapi/vanderbilt-sparql-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vanderbilt.edu
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.vanderbilt.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: apim-portal.app.vanderbilt.edu
  https: false
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: it.vanderbilt.edu
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vanderbilt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vanderbilt University, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vanderbilt University
provider_slug: vanderbilt
slug: vanderbilt-domain-security
source_filename: vanderbilt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vanderbilt.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\n- host: apim-portal.app.vanderbilt.edu\n  https: false\n- host: it.vanderbilt.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: vanderbilt.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vanderbilt/refs/heads/main/security/vanderbilt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- University
- Higher Education
- Education
- Private Research University
- Research Data
- Institutional Repository
- Linked Data
- SPARQL
- Digital Collections
- Television News Archive
- Identity Federation
- Library
- Nashville
- Tennessee
- United States
---
