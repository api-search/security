---
api_specs:
- filename: json-spec
  format: yaml
  label: FoodData Central API
  slug: fooddata-central-api
  spec_type: OpenAPI
  url: https://api.nal.usda.gov/fdc/v1/json-spec?api_key=DEMO_KEY
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:icam_as_notify@ocio.usda.gov"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usda.gov
  spf: true
hosts:
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
name: Fooddata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FoodData Central, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: FoodData Central
provider_slug: fooddata
slug: fooddata-domain-security
source_filename: fooddata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fdc.nal.usda.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nal.usda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:20:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usda.gov\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:icam_as_notify@ocio.usda.gov\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fooddata/refs/heads/main/security/fooddata-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Food
- Nutrition
- USDA
- Government
- Health
- Diet
- Nutrients
- Public Domain
---
