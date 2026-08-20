---
api_specs:
- filename: blueshift-openapi.yml
  format: yaml
  label: Blueshift REST API
  slug: blueshift-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blueshift/refs/heads/main/openapi/blueshift-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blueshift.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getblueshift.com
  spf: true
hosts:
- cert_expires: Oct 23 08:28:08 2026 GMT
  host: blueshift.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 06:07:09 2026 GMT
  host: developer.blueshift.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: api.getblueshift.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Blueshift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blueshift, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blueshift
provider_slug: blueshift
slug: blueshift-domain-security
source_filename: blueshift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blueshift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 08:28:08 2026 GMT\n  hsts: false\n- host: developer.blueshift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 06:07:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getblueshift.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: blueshift.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: getblueshift.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blueshift/refs/heads/main/security/blueshift-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Data Platform
- Customer Engagement
- Marketing Automation
- Cross-Channel Messaging
- Email
- SMS
- Push Notifications
- Segmentation
- Personalization
- Product Recommendations
- Event Tracking
- Product Catalog
- MarTech
- MCP
- agent-native
---
