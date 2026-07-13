---
api_specs:
- filename: sauce.json
  format: json
  label: Sauce Labs Jobs API
  slug: jobs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/sauce.json
- filename: rdc.json
  format: json
  label: Sauce Labs Real Device API
  slug: real-devices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/rdc.json
- filename: real-device-access-api-spec.yaml
  format: yaml
  label: Sauce Labs Real Device Access API
  slug: real-device-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/real-device-access-api-spec.yaml
- filename: accounts.yml
  format: yaml
  label: Sauce Labs Accounts API
  slug: accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/accounts.yml
- filename: buildsv2.json
  format: json
  label: Sauce Labs Builds API
  slug: builds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/buildsv2.json
- filename: test-authoring-api.json
  format: json
  label: Sauce Labs Test Authoring API
  slug: test-authoring
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/test-authoring-api.json
- filename: performance.json
  format: json
  label: Sauce Labs Performance API
  slug: performance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/saucelabs/sauce-docs/refs/heads/main/static/oas/performance.json
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
