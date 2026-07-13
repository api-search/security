---
api_specs:
- filename: agricultural-statistics-service-quickstats-api.yaml
  format: yaml
  label: USDA NASS QuickStats API
  slug: quickstats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agricultural-statistics-service/refs/heads/main/openapi/agricultural-statistics-service-quickstats-api.yaml
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
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gmu.edu
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: www.nass.usda.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: quickstats.nass.usda.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: nassgeodata.gmu.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agricultural Statistics Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agricultural Statistics Service, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Agricultural Statistics Service
provider_slug: agricultural-statistics-service
slug: agricultural-statistics-service-domain-security
source_filename: agricultural-statistics-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nass.usda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: quickstats.nass.usda.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: nassgeodata.gmu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: usda.gov\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:icam_as_notify@ocio.usda.gov\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gmu.edu\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agricultural-statistics-service/refs/heads/main/security/agricultural-statistics-service-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agriculture
- Federal Government
- Statistics
- Open Data
- Geospatial
---
