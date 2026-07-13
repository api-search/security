---
api_specs:
- filename: art-institute-of-chicago-openapi.yml
  format: yaml
  label: Art Institute of Chicago Public API
  slug: art-institute-of-chicago-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/art-institute-of-chicago/refs/heads/main/openapi/art-institute-of-chicago-openapi.yml
description: ''
domains:
- caa:
  - 128 issuewild "trustwave.com"
  - 128 issue "Digicert.com"
  - 128 issue "awstrust.com"
  - 128 issue "globalsign.com"
  - 128 issue "pki.goog"
  - 0 iodef "mailto:networkservices@artic.edu"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: artic.edu
  spf: true
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: api.artic.edu
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 18:44:44 2026 GMT
  host: www.artic.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Art Institute Of Chicago Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Art Institute of Chicago, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Art Institute of Chicago
provider_slug: art-institute-of-chicago
slug: art-institute-of-chicago-domain-security
source_filename: art-institute-of-chicago-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.artic.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: www.artic.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 18:44:44 2026 GMT\n  hsts: false\ndomains:\n- domain: artic.edu\n  dnssec: false\n  caa:\n  - 128 issuewild \"trustwave.com\"\n  - 128 issue \"Digicert.com\"\n  - 128 issue \"awstrust.com\"\n  - 128 issue \"globalsign.com\"\n  - 128 issue \"pki.goog\"\n  - 0 iodef \"mailto:networkservices@artic.edu\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/art-institute-of-chicago/refs/heads/main/security/art-institute-of-chicago-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Art And Design
- Museum
- Open Data
- Cultural Heritage
- IIIF
- Public APIs
- Open Source
---
