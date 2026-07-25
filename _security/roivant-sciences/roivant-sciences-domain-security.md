---
api_specs:
- filename: roivant-sciences-allergies-api-openapi.yml
  format: yaml
  label: Roivant Sciences Allergies API
  slug: roivant-sciences-allergies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-allergies-api-openapi.yml
- filename: roivant-sciences-appointments-api-openapi.yml
  format: yaml
  label: Roivant Sciences Appointments API
  slug: roivant-sciences-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-appointments-api-openapi.yml
- filename: roivant-sciences-diagnoses-api-openapi.yml
  format: yaml
  label: Roivant Sciences Diagnoses API
  slug: roivant-sciences-diagnoses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-diagnoses-api-openapi.yml
- filename: roivant-sciences-documents-api-openapi.yml
  format: yaml
  label: Roivant Sciences Documents API
  slug: roivant-sciences-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-documents-api-openapi.yml
- filename: roivant-sciences-encounters-api-openapi.yml
  format: yaml
  label: Roivant Sciences Encounters API
  slug: roivant-sciences-encounters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-encounters-api-openapi.yml
- filename: roivant-sciences-immunizations-api-openapi.yml
  format: yaml
  label: Roivant Sciences Immunizations API
  slug: roivant-sciences-immunizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-immunizations-api-openapi.yml
- filename: roivant-sciences-labs-api-openapi.yml
  format: yaml
  label: Roivant Sciences Labs API
  slug: roivant-sciences-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-labs-api-openapi.yml
- filename: roivant-sciences-medications-api-openapi.yml
  format: yaml
  label: Roivant Sciences Medications API
  slug: roivant-sciences-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-medications-api-openapi.yml
- filename: roivant-sciences-patients-api-openapi.yml
  format: yaml
  label: Roivant Sciences Patients API
  slug: roivant-sciences-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-patients-api-openapi.yml
- filename: roivant-sciences-practices-api-openapi.yml
  format: yaml
  label: Roivant Sciences Practices API
  slug: roivant-sciences-practices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-practices-api-openapi.yml
- filename: roivant-sciences-procedures-api-openapi.yml
  format: yaml
  label: Roivant Sciences Procedures API
  slug: roivant-sciences-procedures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-procedures-api-openapi.yml
- filename: roivant-sciences-providers-api-openapi.yml
  format: yaml
  label: Roivant Sciences Providers API
  slug: roivant-sciences-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-providers-api-openapi.yml
- filename: roivant-sciences-vitals-api-openapi.yml
  format: yaml
  label: Roivant Sciences Vitals API
  slug: roivant-sciences-vitals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/openapi/roivant-sciences-vitals-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: roivant.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: datavant.com
  spf: true
hosts:
- cert_expires: Aug 20 21:32:37 2026 GMT
  host: roivant.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 02:30:59 2026 GMT
  host: www.datavant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: api.healthjump.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Roivant Sciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roivant Sciences, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Roivant Sciences
provider_slug: roivant-sciences
slug: roivant-sciences-domain-security
source_filename: roivant-sciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: roivant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 21:32:37 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: www.datavant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 02:30:59 2026 GMT\n  hsts: false\n- host: api.healthjump.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: roivant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: datavant.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/security/roivant-sciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Biotech
- Pharmaceutical
- Drug Development
- Clinical Trials
- Health Data
- Tokenization
- Electronic Health Records
- Real World Evidence
- Holding Company
- Healthcare
---
