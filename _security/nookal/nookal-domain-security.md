---
api_specs:
- filename: nookal-openapi.yml
  format: yaml
  label: Nookal Patients API
  slug: nookal-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/openapi/nookal-openapi.yml
- filename: nookal-openapi.yml
  format: yaml
  label: Nookal Appointments API
  slug: nookal-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/openapi/nookal-openapi.yml
- filename: nookal-openapi.yml
  format: yaml
  label: Nookal Clinic API
  slug: nookal-clinic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/openapi/nookal-openapi.yml
- filename: nookal-openapi.yml
  format: yaml
  label: Nookal Invoices API
  slug: nookal-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/openapi/nookal-openapi.yml
- filename: nookal-openapi.yml
  format: yaml
  label: Nookal Verification API
  slug: nookal-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/openapi/nookal-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "starfieldtech.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "starfieldtech.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nookal.com
  spf: true
  spf_record: v=spf1 include:amazonses.com include:_spf.google.com include:mail.zendesk.com include:441562201.spf08.hubspotemail.net ~all
hosts:
- api_live: true
  api_note: https://api.nookal.com/production/v2/verify returns a JSON status envelope; requires api_key.
  cert_expires: Mar 10 01:17:07 2027 GMT
  cert_issuer: GoDaddy.com, Inc.
  host: api.nookal.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  server: Apache
  tls_version: TLSv1.2
- cert_expires: Mar 10 01:17:07 2027 GMT
  cert_issuer: GoDaddy.com, Inc.
  host: www.nookal.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 10886400
  https: true
  server: AmazonS3 via CloudFront
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nookal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nookal, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nookal
provider_slug: nookal
slug: nookal-domain-security
source_filename: nookal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + API hosts\nhosts:\n- host: api.nookal.com\n  https: true\n  tls_version: TLSv1.2\n  cert_issuer: GoDaddy.com, Inc.\n  cert_expires: Mar 10 01:17:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  server: Apache\n  api_live: true\n  api_note: https://api.nookal.com/production/v2/verify returns a JSON status envelope; requires api_key.\n- host: www.nookal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: GoDaddy.com, Inc.\n  cert_expires: Mar 10 01:17:07 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\n  hsts_include_subdomains: true\n  server: AmazonS3 via CloudFront\ndomains:\n- domain: nookal.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"starfieldtech.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0\
  \ issuewild \"letsencrypt.org\"\n  - 0 issuewild \"starfieldtech.com\"\n  spf: true\n  spf_record: v=spf1 include:amazonses.com include:_spf.google.com include:mail.zendesk.com include:441562201.spf08.hubspotemail.net ~all\n  dmarc: true\n  dmarc_policy: reject\nnotes: >-\n  Probes run 2026-07-12. api.nookal.com serves the production REST API over HTTPS\n  with HSTS (max-age 31536000, includeSubDomains) and a GoDaddy-issued certificate;\n  TLS negotiated at 1.2. www.nookal.com is served from Amazon S3 behind CloudFront\n  with HSTS and TLS 1.3. The nookal.com domain publishes SPF and a strict DMARC\n  policy (p=reject) and a CAA record set, but no DNSSEC DS record was found.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/security/nookal-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Practice Management
- Healthcare
- Allied Health
- Appointments
- Scheduling
- Patients
- Clinics
- Bookings
- Physiotherapy
- SaaS
---
