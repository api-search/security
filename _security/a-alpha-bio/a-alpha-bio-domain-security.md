---
api_specs:
- filename: a-alpha-bio-datasets-api-openapi.yml
  format: yaml
  label: A-Alpha Bio Datasets API
  slug: a-alpha-bio-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a-alpha-bio/refs/heads/main/openapi/a-alpha-bio-datasets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aalphabio.com
  spf: true
hosts:
- cert_expires: Oct 30 05:03:46 2026 GMT
  host: www.aalphabio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: atlas.aalphabio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: api.atlas.aalphabio.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: A Alpha Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for A-Alpha Bio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: A-Alpha Bio
provider_slug: a-alpha-bio
slug: a-alpha-bio-domain-security
source_filename: a-alpha-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aalphabio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 05:03:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: atlas.aalphabio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: false\n- host: api.atlas.aalphabio.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: aalphabio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/a-alpha-bio/refs/heads/main/security/a-alpha-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- protein-interactions
- biotechnology
- drug-discovery
- antibody-engineering
- synthetic-biology
- machine-learning
- training-data
- data-licensing
- life-sciences
- Datasets
- protein-design
- bioinformatics
---
