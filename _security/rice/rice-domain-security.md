---
api_specs:
- filename: rice-datasets-api-openapi.yml
  format: yaml
  label: Rice University Datasets API
  slug: rice-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rice/refs/heads/main/openapi/rice-datasets-api-openapi.yml
- filename: rice-reference-api-openapi.yml
  format: yaml
  label: Rice University Reference API
  slug: rice-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rice/refs/heads/main/openapi/rice-reference-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rice.edu
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: internet2.edu
  spf: true
hosts:
- cert_expires: Nov  5 17:31:56 2026 GMT
  host: www.rice.edu
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: idp.rice.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: spaces.at.internet2.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Rice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rice University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rice University
provider_slug: rice
slug: rice-domain-security
source_filename: rice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rice.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 17:31:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: idp.rice.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: null\n- host: spaces.at.internet2.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: rice.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: internet2.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rice/refs/heads/main/security/rice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- University
- Higher Education
- Education
- United States
- Texas
- Private Research University
- Association of American Universities
- Research Data
- Open Data
- Research Repository
- Course Catalog
- Identity Federation
- Library
- Urban Research
---
