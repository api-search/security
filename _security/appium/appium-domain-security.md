---
api_specs:
- filename: appium-server-openapi.yaml
  format: yaml
  label: Appium Server API
  slug: appium-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appium/refs/heads/main/openapi/appium-server-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: appium.io
  spf: true
hosts:
- cert_expires: Oct  3 18:19:44 2026 GMT
  host: appium.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Appium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Appium
provider_slug: appium
slug: appium-domain-security
source_filename: appium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appium.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 18:19:44 2026 GMT\n  hsts: false\ndomains:\n- domain: appium.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appium/refs/heads/main/security/appium-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Android
- Cross-Platform
- iOS
- Mobile Testing
- Open Source
- OpenJS Foundation
- Test Automation
- WebDriver
---
