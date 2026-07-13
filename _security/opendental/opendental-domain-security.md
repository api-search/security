---
api_specs:
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Patients API
  slug: opendental-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Appointments API
  slug: opendental-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Providers API
  slug: opendental-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Procedures API
  slug: opendental-procedures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Insurance & Claims API
  slug: opendental-insurance-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Payments API
  slug: opendental-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Accounts & Ledger API
  slug: opendental-accounts-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Fees & Fee Schedules API
  slug: opendental-fees-feeschedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Recalls API
  slug: opendental-recalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Documents API
  slug: opendental-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Medications & Prescriptions API
  slug: opendental-medications-rx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Referrals API
  slug: opendental-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
- filename: opendental-openapi.yml
  format: yaml
  label: Open Dental Sheets API
  slug: opendental-sheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/openapi/opendental-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opendental.com
  spf: true
hosts:
- cert_expires: Aug 19 14:50:23 2026 GMT
  host: www.opendental.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 14:50:23 2026 GMT
  host: api.opendental.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendental Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Dental, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Open Dental
provider_slug: opendental
slug: opendental-domain-security
source_filename: opendental-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opendental.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 14:50:23 2026 GMT\n  hsts: false\n- host: api.opendental.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 14:50:23 2026 GMT\n  hsts: false\ndomains:\n- domain: opendental.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendental/refs/heads/main/security/opendental-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Dental
- Practice Management
- Healthcare
- EHR
- Patient Records
- REST
---
