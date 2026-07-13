---
api_specs:
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Studies API
  slug: intelerad-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Storage API
  slug: intelerad-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Patients API
  slug: intelerad-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Orders and Worklist API
  slug: intelerad-worklist-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Reports API
  slug: intelerad-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare HL7 Integration API
  slug: intelerad-hl7-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Webhooks and Routing API
  slug: intelerad-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
- filename: intelerad-openapi.yml
  format: yaml
  label: InteleShare Namespaces and Accounts API
  slug: intelerad-namespaces-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/openapi/intelerad-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: intelerad.com
  spf: true
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: dicomgrid.com
  spf: true
hosts:
- cert_expires: Sep 15 01:52:07 2026 GMT
  host: www.intelerad.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: access.dicomgrid.com
  hsts: true
  hsts_max_age: 31550000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intelerad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intelerad, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Intelerad
provider_slug: intelerad
slug: intelerad-domain-security
source_filename: intelerad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.intelerad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:52:07 2026 GMT\n  hsts: false\n- host: access.dicomgrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31550000\ndomains:\n- domain: intelerad.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: dicomgrid.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intelerad/refs/heads/main/security/intelerad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Medical Imaging
- PACS
- Enterprise Imaging
- Radiology
- DICOM
- DICOMweb
- HL7
- FHIR
- Healthcare
- Interoperability
- Image Exchange
---
