---
api_specs:
- filename: sauce-labs-devices-api-openapi.yml
  format: yaml
  label: Sauce Labs Devices API
  slug: sauce-labs-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sauce-labs/refs/heads/main/openapi/sauce-labs-devices-api-openapi.yml
- filename: sauce-labs-job-assets-api-openapi.yml
  format: yaml
  label: Sauce Labs Job Assets API
  slug: sauce-labs-job-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sauce-labs/refs/heads/main/openapi/sauce-labs-job-assets-api-openapi.yml
- filename: sauce-labs-jobs-api-openapi.yml
  format: yaml
  label: Sauce Labs Jobs API
  slug: sauce-labs-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sauce-labs/refs/heads/main/openapi/sauce-labs-jobs-api-openapi.yml
- filename: sauce-labs-platform-api-openapi.yml
  format: yaml
  label: Sauce Labs Platform API
  slug: sauce-labs-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sauce-labs/refs/heads/main/openapi/sauce-labs-platform-api-openapi.yml
- filename: sauce-labs-sessions-api-openapi.yml
  format: yaml
  label: Sauce Labs Sessions API
  slug: sauce-labs-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sauce-labs/refs/heads/main/openapi/sauce-labs-sessions-api-openapi.yml
- filename: sauce-labs-users-api-openapi.yml
  format: yaml
  label: Sauce Labs Users API
  slug: sauce-labs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sauce-labs/refs/heads/main/openapi/sauce-labs-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: saucelabs.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: saucelabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 20:07:48 2026 GMT
  host: docs.saucelabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: api.us-west-1.saucelabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sauce Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sauce Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sauce Labs
provider_slug: sauce-labs
slug: sauce-labs-domain-security
source_filename: sauce-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: saucelabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.saucelabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 20:07:48 2026 GMT\n  hsts: false\n- host: api.us-west-1.saucelabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: saucelabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sauce-labs/refs/heads/main/security/sauce-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Testing
- Cross-Browser Testing
- Mobile Testing
- Real Devices
- Automation
- CI/CD
- Quality Assurance
---
