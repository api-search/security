---
api_specs:
- filename: kartos-therapeutics-content-api-openapi.yml
  format: yaml
  label: Kartos Therapeutics Content API
  slug: kartos-therapeutics-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/openapi/kartos-therapeutics-content-api-openapi.yml
- filename: kartos-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Kartos Therapeutics Discovery API
  slug: kartos-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/openapi/kartos-therapeutics-discovery-api-openapi.yml
- filename: kartos-therapeutics-media-api-openapi.yml
  format: yaml
  label: Kartos Therapeutics Media API
  slug: kartos-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/openapi/kartos-therapeutics-media-api-openapi.yml
- filename: kartos-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Kartos Therapeutics Oembed API
  slug: kartos-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/openapi/kartos-therapeutics-oembed-api-openapi.yml
- filename: kartos-therapeutics-people-api-openapi.yml
  format: yaml
  label: Kartos Therapeutics People API
  slug: kartos-therapeutics-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/openapi/kartos-therapeutics-people-api-openapi.yml
- filename: kartos-therapeutics-science-api-openapi.yml
  format: yaml
  label: Kartos Therapeutics Science API
  slug: kartos-therapeutics-science-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/openapi/kartos-therapeutics-science-api-openapi.yml
- filename: kartos-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Kartos Therapeutics Taxonomy API
  slug: kartos-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/openapi/kartos-therapeutics-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kartosthera.com
  spf: true
- caa:
  - 0 iodef "mailto:caa@wordpress.org"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: kartosthera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 19:43:55 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kartos Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kartos Therapeutics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kartos Therapeutics
provider_slug: kartos-therapeutics
slug: kartos-therapeutics-domain-security
source_filename: kartos-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kartosthera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: kartosthera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kartos-therapeutics/refs/heads/main/security/kartos-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- biotechnology
- pharmaceuticals
- oncology
- hematology
- rare-disease
- precision-medicine
- clinical-trials
- life-sciences
- content-api
---
