---
api_specs:
- filename: dyno-phi-openapi.yml
  format: yaml
  label: Dyno Phi — Protein Design API
  slug: dyno-phi-protein-design-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyno/refs/heads/main/openapi/dyno-phi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dynotx.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dyno-agents.app
  spf: false
hosts:
- cert_expires: Sep 17 03:54:50 2026 GMT
  host: www.dynotx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 12:18:59 2026 GMT
  host: design.dynotx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 15:51:34 2026 GMT
  host: api.dyno-agents.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dyno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dyno, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dyno
provider_slug: dyno
slug: dyno-domain-security
source_filename: dyno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dynotx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 03:54:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: design.dynotx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 12:18:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.dyno-agents.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 15:51:34 2026 GMT\n  hsts: null\ndomains:\n- domain: dynotx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: dyno-agents.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dyno/refs/heads/main/security/dyno-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Gene Therapy
- Genetic Medicine
- Gene Delivery
- AAV Capsid
- Artificial Intelligence
- Machine-Learning
- Drug Discovery
- Healthcare
- Protein Design
- Protein Structure Prediction
- Bioinformatics
- Computational Biology
- Agentic AI
- Life Sciences
---
