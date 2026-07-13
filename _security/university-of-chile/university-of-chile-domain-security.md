---
api_specs:
- filename: university-of-chile-research-data-dataverse.yaml
  format: yaml
  label: UChile Research Data Repository (Dataverse API)
  slug: research-data-dataverse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-chile/refs/heads/main/openapi/university-of-chile-research-data-dataverse.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uchile.cl
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: uchile.cl
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: datos.uchile.cl
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: repositorio.uchile.cl
  https: false
kind: domain-security
layout: security
method: probed
name: University Of Chile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Chile, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Chile
provider_slug: university-of-chile
slug: university-of-chile-domain-security
source_filename: university-of-chile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uchile.cl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: datos.uchile.cl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\n- host: repositorio.uchile.cl\n  https: false\ndomains:\n- domain: uchile.cl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-chile/refs/heads/main/security/university-of-chile-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Data
- Repository
- OAI-PMH
- Dataverse
- Chile
---
