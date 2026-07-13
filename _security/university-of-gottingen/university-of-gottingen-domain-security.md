---
api_specs:
- filename: university-of-gottingen-grodata-rest.yaml
  format: yaml
  label: GRO.data Dataverse REST API
  slug: grodata-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gottingen/refs/heads/main/openapi/university-of-gottingen-grodata-rest.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uni-goettingen.de
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: goettingen-research-online.de
  spf: true
hosts:
- cert_expires: Dec 23 10:32:54 2026 GMT
  host: www.uni-goettingen.de
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 13:27:42 2026 GMT
  host: data.goettingen-research-online.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 30 23:59:59 2026 GMT
  host: guides.dataverse.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Gottingen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Göttingen, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Göttingen
provider_slug: university-of-gottingen
slug: university-of-gottingen-domain-security
source_filename: university-of-gottingen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uni-goettingen.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 10:32:54 2026 GMT\n  hsts: false\n- host: data.goettingen-research-online.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 13:27:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: guides.dataverse.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: uni-goettingen.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: goettingen-research-online.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-gottingen/refs/heads/main/security/university-of-gottingen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Digital Library
- IIIF
- OAI-PMH
- Germany
---
