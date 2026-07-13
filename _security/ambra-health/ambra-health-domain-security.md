---
api_specs:
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Session API
  slug: ambra-health-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Studies API
  slug: ambra-health-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Patients API
  slug: ambra-health-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Users API
  slug: ambra-health-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Groups API
  slug: ambra-health-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Accounts API
  slug: ambra-health-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Namespaces API
  slug: ambra-health-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Sharing API
  slug: ambra-health-sharing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Storage and Images API
  slug: ambra-health-storage-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
- filename: ambra-health-openapi.yml
  format: yaml
  label: Ambra Health Webhooks API
  slug: ambra-health-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/openapi/ambra-health-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "godaddy.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ambrahealth.com
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
- cert_expires: Aug 19 21:03:50 2026 GMT
  host: ambrahealth.com
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
name: Ambra Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ambra Health, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ambra Health
provider_slug: ambra-health
slug: ambra-health-domain-security
source_filename: ambra-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ambrahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 21:03:50 2026 GMT\n  hsts: false\n- host: access.dicomgrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31550000\ndomains:\n- domain: ambrahealth.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: dicomgrid.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambra-health/refs/heads/main/security/ambra-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Medical Imaging
- DICOM
- Healthcare
- PACS
- Image Exchange
- Interoperability
- VNA
- Cloud Imaging
---
