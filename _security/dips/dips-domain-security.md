---
api_specs:
- filename: dips-federation-service-openapi.yml
  format: yaml
  label: DIPS Federation Service
  slug: dips-federation-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-federation-service-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "symantec.com"
  - 0 issue "buypass.no"
  - 0 issue "letsencrypt.org"
  - 0 issue "certainly.com"
  - 0 iodef "mailto:it@dips.no"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dips.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: azure-api.net
  spf: false
hosts:
- cert_expires: Oct 25 19:07:49 2026 GMT
  host: www.dips.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:18:42 2027 GMT
  host: dips.developer.azure-api.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: api.dips.no
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dips Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DIPS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DIPS
provider_slug: dips
slug: dips-domain-security
source_filename: dips-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dips.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 19:07:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dips.developer.azure-api.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:18:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.dips.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dips.com\n  dnssec: true\n  caa:\n  - 0 issue \"symantec.com\"\n  - 0 issue \"buypass.no\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"certainly.com\"\n  - 0 iodef \"mailto:it@dips.no\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure-api.net\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/security/dips-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Electronic Health Records
- Health IT
- FHIR
- openEHR
- Interoperability
- Identity
- OpenID Connect
- Norway
- Hospitals
- SMART on FHIR
---
