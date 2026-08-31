---
api_specs:
- filename: hbku-fanar-api-openapi.yml
  format: yaml
  label: Fanar API
  slug: fanar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-fanar-api-openapi.yml
- filename: hbku-farasa-api-openapi.yml
  format: yaml
  label: Farasa Web API
  slug: farasa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-farasa-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hbku.edu.qa
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fanar.qa
  spf: true
hosts:
- cert_expires: Nov 15 13:42:08 2026 GMT
  host: www.hbku.edu.qa
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 11:12:13 2026 GMT
  host: api.fanar.qa
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 09:58:21 2026 GMT
  host: farasa.qcri.org
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hbku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hamad Bin Khalifa University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hamad Bin Khalifa University
provider_slug: hbku
slug: hbku-domain-security
source_filename: hbku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hbku.edu.qa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 13:42:08 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api.fanar.qa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 11:12:13 2026 GMT\n  hsts: null\n- host: farasa.qcri.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 09:58:21 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: hbku.edu.qa\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: fanar.qa\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/security/hbku-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- Research
- Qatar
- Middle East
- Artificial Intelligence
- Large Language Models
- Natural Language Processing
- Arabic
- Research Computing
- Research Data
- Course Catalog
- Repository
- Open Access
---
