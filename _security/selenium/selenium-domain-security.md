---
api_specs:
- filename: selenium-cookies-api-openapi.yml
  format: yaml
  label: Selenium Cookies API
  slug: selenium-cookies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/selenium/refs/heads/main/openapi/selenium-cookies-api-openapi.yml
- filename: selenium-elements-api-openapi.yml
  format: yaml
  label: Selenium Elements API
  slug: selenium-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/selenium/refs/heads/main/openapi/selenium-elements-api-openapi.yml
- filename: selenium-navigation-api-openapi.yml
  format: yaml
  label: Selenium Navigation API
  slug: selenium-navigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/selenium/refs/heads/main/openapi/selenium-navigation-api-openapi.yml
- filename: selenium-script-api-openapi.yml
  format: yaml
  label: Selenium Script API
  slug: selenium-script-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/selenium/refs/heads/main/openapi/selenium-script-api-openapi.yml
- filename: selenium-session-api-openapi.yml
  format: yaml
  label: Selenium Session API
  slug: selenium-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/selenium/refs/heads/main/openapi/selenium-session-api-openapi.yml
- filename: selenium-status-api-openapi.yml
  format: yaml
  label: Selenium Status API
  slug: selenium-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/selenium/refs/heads/main/openapi/selenium-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: selenium.dev
  spf: true
hosts:
- cert_expires: Nov 19 17:58:08 2026 GMT
  host: www.selenium.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Selenium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Selenium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Selenium
provider_slug: selenium
slug: selenium-domain-security
source_filename: selenium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.selenium.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 17:58:08 2026 GMT\n  hsts: false\ndomains:\n- domain: selenium.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/selenium/refs/heads/main/security/selenium-domain-security.yml
summary_line: TLSv1.3
tags:
- Automation
- Browsers
- End-to-End Testing
- Quality Assurance
- Testing
- WebDriver
---
