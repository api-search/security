---
api_specs:
- filename: natural-resources-conservation-service-openapi.yml
  format: yaml
  label: NRCS Soil Data Access
  slug: soil-data-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natural-resources-conservation-service/refs/heads/main/openapi/natural-resources-conservation-service-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:icam_as_notify@ocio.usda.gov"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usda.gov
  spf: true
hosts:
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: www.nrcs.usda.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: sdmdataaccess.nrcs.usda.gov
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: sdmdataaccess.sc.egov.usda.gov
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Natural Resources Conservation Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Natural Resources Conservation Service, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Natural Resources Conservation Service
provider_slug: natural-resources-conservation-service
slug: natural-resources-conservation-service-domain-security
source_filename: natural-resources-conservation-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nrcs.usda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\n- host: sdmdataaccess.nrcs.usda.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\n- host: sdmdataaccess.sc.egov.usda.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: usda.gov\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:icam_as_notify@ocio.usda.gov\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natural-resources-conservation-service/refs/heads/main/security/natural-resources-conservation-service-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Agriculture
- Conservation
- Soil
- Natural Resources
---
