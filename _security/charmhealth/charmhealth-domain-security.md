---
api_specs:
- filename: charmhealth-fhir-api-openapi.yml
  format: yaml
  label: CharmHealth FHIR API
  slug: fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-fhir-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: charmhealth.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: charmtracker.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.charmhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: ehr2.charmtracker.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Charmhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CharmHealth, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CharmHealth
provider_slug: charmhealth
slug: charmhealth-domain-security
source_filename: charmhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.charmhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: false\n- host: ehr2.charmtracker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: charmhealth.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: charmtracker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/security/charmhealth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- EHR
- EMR
- FHIR
- Healthcare
- HL7
- Patient Engagement
- Patients
- SMART on FHIR
- US Core
---
