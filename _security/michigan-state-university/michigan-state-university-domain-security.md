---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: MSU Libraries Catalog REST API (VuFind)
  slug: catalog-rest
  spec_type: OpenAPI
  url: https://catalog.lib.msu.edu/api/v1/?swagger
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: msu.edu
  spf: true
hosts:
- cert_expires: Sep 24 17:52:26 2026 GMT
  host: www.msu.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 20:08:41 2026 GMT
  host: catalog.lib.msu.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: d.lib.msu.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Michigan State University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Michigan State University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Michigan State University
provider_slug: michigan-state-university
slug: michigan-state-university-domain-security
source_filename: michigan-state-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.msu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:52:26 2026 GMT\n  hsts: false\n- host: catalog.lib.msu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:08:41 2026 GMT\n  hsts: false\n- host: d.lib.msu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: msu.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/michigan-state-university/refs/heads/main/security/michigan-state-university-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Library
- Open Data
- Metadata
- United States
- Michigan
---
