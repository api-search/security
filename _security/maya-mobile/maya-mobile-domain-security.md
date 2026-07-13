---
api_specs:
- filename: maya-mobile-openapi.yml
  format: yaml
  label: Maya Mobile Plans and Products API
  slug: plans-products
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-openapi.yml
- filename: maya-mobile-openapi.yml
  format: yaml
  label: Maya Mobile eSIMs and Provisioning API
  slug: esims-provisioning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-openapi.yml
- filename: maya-mobile-openapi.yml
  format: yaml
  label: Maya Mobile Usage and Topup API
  slug: usage-topup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-openapi.yml
- filename: maya-mobile-openapi.yml
  format: yaml
  label: Maya Mobile Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-openapi.yml
- filename: maya-mobile-openapi.yml
  format: yaml
  label: Maya Mobile Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-openapi.yml
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
