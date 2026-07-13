---
api_specs:
- filename: rest.apidoc.blueconic.com
  format: yaml
  label: BlueConic REST API v2
  slug: blueconic-rest-api-v2
  spec_type: OpenAPI
  url: https://rest.apidoc.blueconic.com
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:admin@blueconic.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blueconic.com
  spf: true
hosts:
- cert_expires: Sep 16 18:59:01 2026 GMT
  host: www.blueconic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 06:54:24 2026 GMT
  host: support.blueconic.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blueconic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlueConic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BlueConic
provider_slug: blueconic
slug: blueconic-domain-security
source_filename: blueconic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blueconic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 18:59:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.blueconic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:54:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: blueconic.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:admin@blueconic.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blueconic/refs/heads/main/security/blueconic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Data Platform
- CDP
- Customer Profiles
- Segments
- Data Activation
- First-Party Data
- Lifecycle Stages
- Connections
- Privacy
---
