---
api_specs:
- filename: ceros-accounts-api-openapi.yml
  format: yaml
  label: Ceros Accounts API
  slug: ceros-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-accounts-api-openapi.yml
- filename: ceros-embedcodes-api-openapi.yml
  format: yaml
  label: Ceros Embed Codes API
  slug: ceros-embedcodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-embedcodes-api-openapi.yml
- filename: ceros-experience-api-openapi.yml
  format: yaml
  label: Ceros Experience API
  slug: ceros-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-experience-api-openapi.yml
- filename: ceros-experiencepage-api-openapi.yml
  format: yaml
  label: Ceros Experience Page API
  slug: ceros-experiencepage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-experiencepage-api-openapi.yml
- filename: ceros-folders-api-openapi.yml
  format: yaml
  label: Ceros Folders API
  slug: ceros-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-folders-api-openapi.yml
- filename: ceros-oembed-api-openapi.yml
  format: yaml
  label: Ceros Oembed API
  slug: ceros-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-oembed-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
- caa:
  - 0 iodef "mailto:domains@ceros.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ceros.com
  spf: true
hosts:
- cert_expires: Oct 19 20:15:48 2026 GMT
  host: forgeglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 18:57:09 2026 GMT
  host: view.ceros.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 17:57:54 2026 GMT
  host: rest.ceros.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ceros Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ceros, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ceros
provider_slug: ceros
slug: ceros-domain-security
source_filename: ceros-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 20:15:48 2026 GMT\n  hsts: null\n- host: view.ceros.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 18:57:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: rest.ceros.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 17:57:54 2026 GMT\n  hsts: null\ndomains:\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: ceros.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:domains@ceros.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/security/ceros-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Content Management
- Interactive Content
- Digital Experience
- Embed
- oEmbed
- CMS Integration
- Marketing
- Design
- No Code
- Content Delivery
- Media and Publishing
- SDK
---
