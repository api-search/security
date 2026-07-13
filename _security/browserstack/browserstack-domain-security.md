---
api_specs:
- filename: browserstack-openapi.yml
  format: yaml
  label: BrowserStack
  slug: browserstack
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserstack/refs/heads/main/openapi/browserstack-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: browserstack.com
  spf: true
hosts:
- cert_expires: Jul 29 06:21:55 2026 GMT
  host: www.browserstack.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 29 06:21:55 2026 GMT
  host: api.browserstack.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Browserstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BrowserStack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BrowserStack
provider_slug: browserstack
slug: browserstack-domain-security
source_filename: browserstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.browserstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 06:21:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.browserstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 06:21:55 2026 GMT\n  hsts: null\ndomains:\n- domain: browserstack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/browserstack/refs/heads/main/security/browserstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accessibility
- Appium
- Applications
- Automation
- CI/CD
- Cross-Browser Testing
- Enterprise
- JavaScript
- Low Code
- Mobile Testing
- QA
- Regression Testing
- Selenium
- Testing
- Unit Testing
- Visual Testing
---
