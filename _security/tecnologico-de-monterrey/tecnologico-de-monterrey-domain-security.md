---
api_specs:
- filename: tecnologico-de-monterrey-datahub-rest.yaml
  format: yaml
  label: Tec de Monterrey Dataverse Native REST API
  slug: datahub-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tecnologico-de-monterrey/refs/heads/main/openapi/tecnologico-de-monterrey-datahub-rest.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tec.mx
  spf: true
hosts:
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: tec.mx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: datahub.tec.mx
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 29 23:59:59 2026 GMT
  host: repositorio.tec.mx
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tecnologico De Monterrey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tecnológico de Monterrey, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tecnológico de Monterrey
provider_slug: tecnologico-de-monterrey
slug: tecnologico-de-monterrey-domain-security
source_filename: tecnologico-de-monterrey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tec.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: datahub.tec.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: false\n- host: repositorio.tec.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tec.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tecnologico-de-monterrey/refs/heads/main/security/tecnologico-de-monterrey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Open Data
- Research Data
- Mexico
- Dataverse
- OAI-PMH
---
