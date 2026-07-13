---
api_specs:
- filename: index.html
  format: yaml
  label: LambdaTest Web Automation API
  slug: web-automation-api
  spec_type: OpenAPI
  url: https://swagger-api-support.lambdatest.com/index.html
- filename: index.html
  format: yaml
  label: LambdaTest SmartUI API
  slug: smartui-api
  spec_type: OpenAPI
  url: https://swagger-api-support.lambdatest.com/smartui/index.html
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lambdatest.com
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: www.lambdatest.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.lambdatest.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: mobile-api.lambdatest.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lambdatest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LambdaTest, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LambdaTest
provider_slug: lambdatest
slug: lambdatest-domain-security
source_filename: lambdatest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lambdatest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\n- host: api.lambdatest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\n- host: mobile-api.lambdatest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: lambdatest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lambdatest/refs/heads/main/security/lambdatest-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Testing
- Cross-Browser Testing
- Selenium
- Cypress
- Playwright
- Mobile Testing
- Automation
- QA
- Visual Regression
---
