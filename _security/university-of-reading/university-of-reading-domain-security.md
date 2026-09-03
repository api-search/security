---
api_specs:
- filename: university-of-reading-centaur-oai-pmh-openapi.yml
  format: yaml
  label: CentAUR OAI-PMH Metadata API
  slug: centaur-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-reading/refs/heads/main/openapi/university-of-reading-centaur-oai-pmh-openapi.yml
- filename: university-of-reading-research-data-archive-oai-pmh-openapi.yml
  format: yaml
  label: Research Data Archive OAI-PMH Metadata API
  slug: research-data-archive-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-reading/refs/heads/main/openapi/university-of-reading-research-data-archive-oai-pmh-openapi.yml
- filename: university-of-reading-eprints-rest-openapi.yml
  format: yaml
  label: CentAUR Repository REST Listings
  slug: centaur-eprints-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-reading/refs/heads/main/openapi/university-of-reading-eprints-rest-openapi.yml
- filename: university-of-reading-eprints-rest-openapi.yml
  format: yaml
  label: Research Data Archive REST Listings
  slug: research-data-archive-eprints-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-reading/refs/heads/main/openapi/university-of-reading-eprints-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reading.ac.uk
  spf: true
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: www.reading.ac.uk
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: centaur.reading.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: researchdata.reading.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Reading Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Reading, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Reading
provider_slug: university-of-reading
slug: university-of-reading-domain-security
source_filename: university-of-reading-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reading.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: centaur.reading.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: researchdata.reading.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reading.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-reading/refs/heads/main/security/university-of-reading-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- Research
- Research Repository
- Research Data
- Open Access
- OAI-PMH
- Metadata
- Identity Federation
- Course Catalog
- Library
- Climate Data
- United Kingdom
- England
---
