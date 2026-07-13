---
api_specs:
- filename: llms.txt
  format: yaml
  label: Smartlook REST API
  slug: smartlook-rest-api
  spec_type: OpenAPI
  url: https://integrations.smartlook.com/llms.txt
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smartlook.com
  spf: true
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: false
  dnssec: false
  domain: smartlook.cloud
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: www.smartlook.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 19:10:39 2026 GMT
  host: integrations.smartlook.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: api.eu.smartlook.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smartlook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smartlook, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Smartlook
provider_slug: smartlook
slug: smartlook-domain-security
source_filename: smartlook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smartlook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: integrations.smartlook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:10:39 2026 GMT\n  hsts: null\n- host: api.eu.smartlook.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: smartlook.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: smartlook.cloud\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n\
  \  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartlook/refs/heads/main/security/smartlook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Product Analytics
- Session Recording
- Heatmaps
- Funnels
- User Behavior
- Event Tracking
- Visitor Analytics
- Digital Experience
---
