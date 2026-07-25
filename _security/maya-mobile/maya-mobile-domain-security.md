---
api_specs:
- filename: maya-mobile-esims-api-openapi.yml
  format: yaml
  label: Maya Mobile eSIMs API
  slug: maya-mobile-esims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-esims-api-openapi.yml
- filename: maya-mobile-orders-api-openapi.yml
  format: yaml
  label: Maya Mobile Orders API
  slug: maya-mobile-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-orders-api-openapi.yml
- filename: maya-mobile-plans-api-openapi.yml
  format: yaml
  label: Maya Mobile Plans API
  slug: maya-mobile-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-plans-api-openapi.yml
- filename: maya-mobile-usage-api-openapi.yml
  format: yaml
  label: Maya Mobile Usage API
  slug: maya-mobile-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: maya.net
  spf: true
hosts:
- cert_expires: Oct  7 18:29:20 2026 GMT
  host: maya.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: api.maya.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maya Mobile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maya Mobile, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Maya Mobile
provider_slug: maya-mobile
slug: maya-mobile-domain-security
source_filename: maya-mobile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maya.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 18:29:20 2026 GMT\n  hsts: false\n- host: api.maya.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: maya.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/security/maya-mobile-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- eSIM
- Connectivity
- Mobile Data
- Roaming
- Telecom
---
