---
api_specs:
- filename: canvas-medical-fhir-api-openapi.yml
  format: yaml
  label: Canvas Medical FHIR API
  slug: canvas-medical-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-medical/refs/heads/main/openapi/canvas-medical-fhir-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: canvasmedical.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:infrastructure-staff@python.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: pypi.org
  spf: true
hosts:
- cert_expires: Sep 18 03:17:29 2026 GMT
  host: www.canvasmedical.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: docs.canvasmedical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 04:33:07 2027 GMT
  host: pypi.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Canvas Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canvas Medical, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Canvas Medical
provider_slug: canvas-medical
slug: canvas-medical-domain-security
source_filename: canvas-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.canvasmedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 03:17:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.canvasmedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: false\n- host: pypi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 04:33:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: canvasmedical.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pypi.org\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:infrastructure-staff@python.org\"\
  \n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canvas-medical/refs/heads/main/security/canvas-medical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- EHR
- FHIR
- Healthcare
- Electronic Health Records
- Virtual Care
- Clinical Workflows
- Patient Management
- Care Coordination
---
