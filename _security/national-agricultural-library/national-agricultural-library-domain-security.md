---
api_specs:
- filename: national-agricultural-library-openapi.json
  format: json
  label: USDA FoodData Central API
  slug: fooddata-central
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-agricultural-library/main/openapi/national-agricultural-library-openapi.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:icam_as_notify@ocio.usda.gov"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usda.gov
  spf: true
hosts:
- cert_expires: Aug 10 23:59:59 2026 GMT
  host: www.nal.usda.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 10 23:59:59 2026 GMT
  host: fdc.nal.usda.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 25 19:20:59 2026 GMT
  host: api.nal.usda.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Agricultural Library Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Agricultural Library, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Agricultural Library
provider_slug: national-agricultural-library
slug: national-agricultural-library-domain-security
source_filename: national-agricultural-library-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nal.usda.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fdc.nal.usda.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nal.usda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:20:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usda.gov\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:icam_as_notify@ocio.usda.gov\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-agricultural-library/refs/heads/main/security/national-agricultural-library-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Agriculture
- Federal Government
- Library
- Food
- Nutrition
---
