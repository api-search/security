---
api_specs:
- filename: foreign-agricultural-service-openapi.yml
  format: yaml
  label: USDA FAS Open Data API
  slug: fas-open-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foreign-agricultural-service/refs/heads/main/openapi/foreign-agricultural-service-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:icam_as_notify@ocio.usda.gov"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usda.gov
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.fas.usda.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: apps.fas.usda.gov
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Foreign Agricultural Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foreign Agricultural Service, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Foreign Agricultural Service
provider_slug: foreign-agricultural-service
slug: foreign-agricultural-service-domain-security
source_filename: foreign-agricultural-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fas.usda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\n- host: apps.fas.usda.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: usda.gov\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:icam_as_notify@ocio.usda.gov\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foreign-agricultural-service/refs/heads/main/security/foreign-agricultural-service-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Agriculture
- Federal Government
---
