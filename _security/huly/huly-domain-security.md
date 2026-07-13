---
api_specs:
- filename: huly-openapi.yml
  format: yaml
  label: Huly Platform SDK
  slug: huly-platform-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huly/refs/heads/main/openapi/huly-openapi.yml
- filename: huly-openapi.yml
  format: yaml
  label: Huly Cloud
  slug: huly-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huly/refs/heads/main/openapi/huly-openapi.yml
- filename: huly-openapi.yml
  format: yaml
  label: Huly Tracker
  slug: huly-tracker
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huly/refs/heads/main/openapi/huly-openapi.yml
- filename: huly-openapi.yml
  format: yaml
  label: Huly Documents
  slug: huly-documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huly/refs/heads/main/openapi/huly-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: huly.io
  spf: true
hosts:
- cert_expires: Sep 16 10:02:15 2026 GMT
  host: huly.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Huly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Huly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Huly
provider_slug: huly
slug: huly-domain-security
source_filename: huly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: huly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 10:02:15 2026 GMT\n  hsts: false\ndomains:\n- domain: huly.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huly/refs/heads/main/security/huly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Project Management
- Collaboration
- Open Source
- Productivity
- SDK
---
