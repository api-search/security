---
api_specs:
- filename: genialis-about-api-openapi.yml
  format: yaml
  label: Genialis About API
  slug: genialis-about-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genialis/refs/heads/main/openapi/genialis-about-api-openapi.yml
- filename: genialis-api-api-openapi.yml
  format: yaml
  label: Genialis API
  slug: genialis-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genialis/refs/heads/main/openapi/genialis-api-api-openapi.yml
- filename: genialis-health-check-api-openapi.yml
  format: yaml
  label: Genialis Health Check API
  slug: genialis-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genialis/refs/heads/main/openapi/genialis-health-check-api-openapi.yml
- filename: genialis-rest-auth-api-openapi.yml
  format: yaml
  label: Genialis Rest Auth API
  slug: genialis-rest-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genialis/refs/heads/main/openapi/genialis-rest-auth-api-openapi.yml
- filename: genialis-saml-auth-api-openapi.yml
  format: yaml
  label: Genialis Saml Auth API
  slug: genialis-saml-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genialis/refs/heads/main/openapi/genialis-saml-auth-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: genialis.com
  spf: true
hosts:
- cert_expires: Oct 24 16:41:27 2026 GMT
  host: www.genialis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: docs.genialis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: app.genialis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Genialis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genialis, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Genialis
provider_slug: genialis
slug: genialis-domain-security
source_filename: genialis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.genialis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 16:41:27 2026 GMT\n  hsts: false\n- host: docs.genialis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: false\n- host: app.genialis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: genialis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genialis/refs/heads/main/security/genialis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Bioinformatics
- Precision Medicine
- Genomics
- Life Sciences
- Healthcare
- Machine Learning
- Artificial Intelligence
- Multiomics
- Oncology
- Data Platform
- Open Source
---
