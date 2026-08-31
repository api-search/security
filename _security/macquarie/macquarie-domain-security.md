---
api_specs:
- filename: macquarie-research-portal-oai-pmh-openapi.yml
  format: yaml
  label: Macquarie University Research Portal OAI-PMH
  slug: research-portal-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/openapi/macquarie-research-portal-oai-pmh-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mq.edu.au
  spf: true
hosts:
- cert_expires: Nov 18 11:52:37 2026 GMT
  host: www.mq.edu.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 06:59:38 2026 GMT
  host: research-management.mq.edu.au
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: idp.mq.edu.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Macquarie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Macquarie University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Macquarie University
provider_slug: macquarie
slug: macquarie-domain-security
source_filename: macquarie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "# authorship: written by API Evangelist from live DNS/TLS/HTTP probes of this repo's hosts.\n# x-method: derived\ngenerated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mq.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 11:52:37 2026 GMT\n  hsts: null\n- host: research-management.mq.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 06:59:38 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: idp.mq.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mq.edu.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macquarie/refs/heads/main/security/macquarie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- Australia
- Group of Eight Peer
- Research Data
- Research Repository
- Metadata Harvesting
- OAI-PMH
- Identity Federation
- Library
- Course Catalog
---
