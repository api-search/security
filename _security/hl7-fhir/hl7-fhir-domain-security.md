---
api_specs:
- filename: hl7-fhir-r4-openapi.yml
  format: yaml
  label: HL7 FHIR R4 Healthcare API
  slug: hl7-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hl7-fhir/refs/heads/main/openapi/hl7-fhir-r4-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "symantec.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hl7.org
  spf: true
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: www.hl7.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: hl7.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hl7 Fhir Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HL7 FHIR, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HL7 FHIR
provider_slug: hl7-fhir
slug: hl7-fhir-domain-security
source_filename: hl7-fhir-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hl7.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\n- host: hl7.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: hl7.org\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"symantec.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hl7-fhir/refs/heads/main/security/hl7-fhir-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Clinical
- FHIR
- Healthcare
- HL7
- Interoperability
---
