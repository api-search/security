---
api_specs:
- filename: wageningen-university-research-agrodatacube-v2.yaml
  format: yaml
  label: AgroDataCube API v2
  slug: agrodatacube-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wageningen-university-research/refs/heads/main/openapi/wageningen-university-research-agrodatacube-v2.yaml
- filename: wageningen-university-research-agrodatacube-v1.yaml
  format: yaml
  label: AgroDataCube API v1 (legacy)
  slug: agrodatacube-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wageningen-university-research/refs/heads/main/openapi/wageningen-university-research-agrodatacube-v1.yaml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 iodef "mailto:servicedesk.it@wur.nl"
  - 0 issue "harica.gr"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wur.nl
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: azure-api.net
  spf: false
hosts:
- cert_expires: Dec 21 12:19:46 2026 GMT
  host: www.wur.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 15:42:18 2026 GMT
  host: agrodatacube.wur.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 07:51:50 2026 GMT
  host: euw-apim-fism-001-p.developer.azure-api.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wageningen University Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wageningen University & Research, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wageningen University & Research
provider_slug: wageningen-university-research
slug: wageningen-university-research-domain-security
source_filename: wageningen-university-research-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wur.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 12:19:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: agrodatacube.wur.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 15:42:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: euw-apim-fism-001-p.developer.azure-api.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 07:51:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wur.nl\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 iodef \"mailto:servicedesk.it@wur.nl\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure-api.net\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wageningen-university-research/refs/heads/main/security/wageningen-university-research-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Agriculture
- Agri-Food
- Open Data
- Netherlands
---
