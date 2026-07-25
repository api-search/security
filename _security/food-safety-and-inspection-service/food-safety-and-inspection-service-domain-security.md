---
api_specs:
- filename: food-safety-and-inspection-service-recalls-api-openapi.yml
  format: yaml
  label: Food Safety and Inspection Service Recalls API
  slug: food-safety-and-inspection-service-recalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-safety-and-inspection-service/refs/heads/main/openapi/food-safety-and-inspection-service-recalls-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:icam_as_notify@ocio.usda.gov"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usda.gov
  spf: true
hosts:
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: www.fsis.usda.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Food Safety And Inspection Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Food Safety and Inspection Service, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Food Safety and Inspection Service
provider_slug: food-safety-and-inspection-service
slug: food-safety-and-inspection-service-domain-security
source_filename: food-safety-and-inspection-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fsis.usda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: usda.gov\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:icam_as_notify@ocio.usda.gov\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/food-safety-and-inspection-service/refs/heads/main/security/food-safety-and-inspection-service-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Food
- Food Safety
- Inspections
- Recalls
- Meat
- Poultry
- Eggs
---
