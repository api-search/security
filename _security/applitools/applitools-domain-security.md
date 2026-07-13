---
api_specs:
- filename: applitools-openapi.yml
  format: yaml
  label: Applitools Eyes Server REST API
  slug: eyes-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applitools/refs/heads/main/openapi/applitools-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: applitools.com
  spf: true
hosts:
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: applitools.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: eyesapi.applitools.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: eyes.applitools.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Applitools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Applitools, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Applitools
provider_slug: applitools
slug: applitools-domain-security
source_filename: applitools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: applitools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: false\n- host: eyesapi.applitools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\n- host: eyes.applitools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: applitools.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/applitools/refs/heads/main/security/applitools-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Testing
- Visual AI
- Visual Testing
- Autonomous Testing
- REST
- SDK
- Cross-Browser
- Execution Cloud
---
