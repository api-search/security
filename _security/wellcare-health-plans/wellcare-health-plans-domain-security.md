---
api_specs:
- filename: wellcare-fhir-patient-access-api-openapi.yml
  format: yaml
  label: WellCare FHIR Patient Access API
  slug: fhir-patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-fhir-patient-access-api-openapi.yml
- filename: wellcare-fhir-provider-directory-api-openapi.yml
  format: yaml
  label: WellCare FHIR Provider Directory API
  slug: fhir-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-fhir-provider-directory-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wellcare.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: centene.com
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.wellcare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: partners.centene.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wellcare Health Plans Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for wellcare-health-plans, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: wellcare-health-plans
provider_slug: wellcare-health-plans
slug: wellcare-health-plans-domain-security
source_filename: wellcare-health-plans-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wellcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partners.centene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wellcare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: centene.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/security/wellcare-health-plans-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
---
