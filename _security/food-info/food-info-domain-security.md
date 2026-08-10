---
api_specs:
- filename: food-info-apiv1-api-openapi.yml
  format: yaml
  label: Food Info API V1 API
  slug: food-info-apiv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-info/refs/heads/main/openapi/food-info-apiv1-api-openapi.yml
- filename: food-info-recipesapi-api-openapi.yml
  format: yaml
  label: Food Info Recipes API API
  slug: food-info-recipesapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/food-info/refs/heads/main/openapi/food-info-recipesapi-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: food-info.org
  spf: true
hosts:
- cert_expires: Oct 22 14:04:23 2026 GMT
  host: food-info.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  security_headers:
    permissions-policy: camera=(), microphone=(), geolocation=(), interest-cohort=()
    referrer-policy: no-referrer
    x-content-type-options: nosniff
    x-frame-options: SAMEORIGIN
  tls_version: TLSv1.3
- cert_expires: Oct 22 14:04:23 2026 GMT
  host: api.food-info.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  security_headers:
    cross-origin-resource-policy: same-site
    permissions-policy: camera=(), microphone=(), geolocation=()
    referrer-policy: strict-origin-when-cross-origin
    x-content-type-options: nosniff
    x-frame-options: DENY
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Food Info Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Food Info, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Food Info
provider_slug: food-info
slug: food-info-domain-security
source_filename: food-info-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: food-info.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 14:04:23 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  security_headers:\n    x-content-type-options: nosniff\n    x-frame-options: SAMEORIGIN\n    referrer-policy: no-referrer\n    permissions-policy: camera=(), microphone=(), geolocation=(), interest-cohort=()\n- host: api.food-info.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 14:04:23 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  security_headers:\n    x-content-type-options: nosniff\n    x-frame-options: DENY\n    referrer-policy: strict-origin-when-cross-origin\n    permissions-policy: camera=(), microphone=(), geolocation=()\n    cross-origin-resource-policy: same-site\ndomains:\n- domain: food-info.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nx-evidence:\n\
  \  fetched: '2026-08-04'\n  note: >-\n    HSTS and the response security headers were re-observed directly on 2026-08-04 with a live GET\n    (https://food-info.org/robots.txt and https://api.food-info.org/api/v1/nutrients). The scripted\n    HEAD probe recorded hsts: null because both hosts sit behind a Cloudflare managed challenge that\n    rejects non-browser HEAD requests; the values above supersede it.\n  hosts_edge: cloudflare in front of fly.io\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/food-info/refs/heads/main/security/food-info-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Nutrition
- Food
- Food Composition
- Nutrients
- Data
- Open Data
- Dietetics
- Recipes
- Health
- Research
---
