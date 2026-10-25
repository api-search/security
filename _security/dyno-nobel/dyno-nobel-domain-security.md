---
api_specs:
- filename: dyno-nobel-robotslandingpage-api-openapi.yml
  format: yaml
  label: Dyno Nobel Robots Landing Page API
  slug: dyno-nobel-robotslandingpage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyno-nobel/refs/heads/main/openapi/dyno-nobel-robotslandingpage-api-openapi.yml
- filename: dyno-nobel-robotstext-api-openapi.yml
  format: yaml
  label: Dyno Nobel Robots Text API
  slug: dyno-nobel-robotstext-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyno-nobel/refs/heads/main/openapi/dyno-nobel-robotstext-api-openapi.yml
- filename: dyno-nobel-searchapi-api-openapi.yml
  format: yaml
  label: Dyno Nobel Search API
  slug: dyno-nobel-searchapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyno-nobel/refs/heads/main/openapi/dyno-nobel-searchapi-api-openapi.yml
- filename: dyno-nobel-sitemanifest-api-openapi.yml
  format: yaml
  label: Dyno Nobel Site Manifest API
  slug: dyno-nobel-sitemanifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyno-nobel/refs/heads/main/openapi/dyno-nobel-sitemanifest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dynonobel.com
  spf: true
hosts:
- cert_expires: Jan 10 05:18:31 2027 GMT
  host: www.dynonobel.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dyno Nobel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dyno Nobel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dyno Nobel
provider_slug: dyno-nobel
slug: dyno-nobel-domain-security
source_filename: dyno-nobel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dynonobel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 05:18:31 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: dynonobel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dyno-nobel/refs/heads/main/security/dyno-nobel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Explosives
- Mining
- Industrial Manufacturing
- Blasting
- Australia
---
