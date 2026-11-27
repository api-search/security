---
api_specs:
- filename: onefindme-com-search-api-openapi.yml
  format: yaml
  label: OneFindMe Search API
  slug: onefindme-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onefindme-com/openapi/onefindme-com-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: onefindme.com
  spf: true
hosts:
- cert_expires: Jan 14 20:43:22 2027 GMT
  host: onefindme.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OneFindMe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneFindMe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OneFindMe
provider_slug: onefindme-com
slug: onefindme-com-domain-security
source_filename: onefindme-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onefindme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 20:43:22 2027 GMT\n  hsts: false\ndomains:\n- domain: onefindme.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/onefindme-com/security/onefindme-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Search
- E-Commerce
- Affiliates
- Multilingual
- Tools
---
