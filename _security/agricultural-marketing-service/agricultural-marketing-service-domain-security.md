---
api_specs:
- filename: agricultural-marketing-service-mars-api.yaml
  format: yaml
  label: USDA AMS MARS API (MyMarketNews)
  slug: usda-ams-mars-api-mymarketnews
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/openapi/agricultural-marketing-service-mars-api.yaml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:icam_as_notify@ocio.usda.gov"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usda.gov
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: www.ams.usda.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: mymarketnews.ams.usda.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: marsapi.ams.usda.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agricultural Marketing Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agricultural Marketing Service, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Agricultural Marketing Service
provider_slug: agricultural-marketing-service
slug: agricultural-marketing-service-domain-security
source_filename: agricultural-marketing-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ams.usda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mymarketnews.ams.usda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\n- host: marsapi.ams.usda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: usda.gov\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:icam_as_notify@ocio.usda.gov\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agricultural-marketing-service/refs/heads/main/security/agricultural-marketing-service-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agriculture
- Federal Government
- Market News
- Livestock
- Dairy
- Fruits And Vegetables
- Cotton
- Tobacco
---
