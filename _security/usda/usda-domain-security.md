---
api_specs:
- filename: fdc_api.html
  format: yaml
  label: USDA FoodData Central API
  slug: usda-fooddata-central-api
  spec_type: OpenAPI
  url: https://fdc.nal.usda.gov/api-spec/fdc_api.html
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
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.usda.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
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
name: Usda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for USDA, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: USDA
provider_slug: usda
slug: usda-domain-security
source_filename: usda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\n- host: fdc.nal.usda.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nal.usda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:20:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usda.gov\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:icam_as_notify@ocio.usda.gov\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usda/refs/heads/main/security/usda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agriculture
- Food Safety
- Nutrition
- Statistics
- Geospatial
- Market News
- Federal Government
---
