---
api_specs:
- filename: bugbug-io-components-api-openapi.yml
  format: yaml
  label: BugBug Components API
  slug: bugbug-io-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-components-api-openapi.yml
- filename: bugbug-io-config-api-openapi.yml
  format: yaml
  label: BugBug Config API
  slug: bugbug-io-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-config-api-openapi.yml
- filename: bugbug-io-folders-api-openapi.yml
  format: yaml
  label: BugBug Folders API
  slug: bugbug-io-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-folders-api-openapi.yml
- filename: bugbug-io-groups-api-openapi.yml
  format: yaml
  label: BugBug Groups API
  slug: bugbug-io-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-groups-api-openapi.yml
- filename: bugbug-io-import-export-api-openapi.yml
  format: yaml
  label: BugBug Import / Export API
  slug: bugbug-io-import-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-import-export-api-openapi.yml
- filename: bugbug-io-organizations-api-openapi.yml
  format: yaml
  label: BugBug Organizations API
  slug: bugbug-io-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-organizations-api-openapi.yml
- filename: bugbug-io-profiles-api-openapi.yml
  format: yaml
  label: BugBug Profiles API
  slug: bugbug-io-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-profiles-api-openapi.yml
- filename: bugbug-io-projects-api-openapi.yml
  format: yaml
  label: BugBug Projects API
  slug: bugbug-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-projects-api-openapi.yml
- filename: bugbug-io-settings-api-openapi.yml
  format: yaml
  label: BugBug Settings API
  slug: bugbug-io-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-settings-api-openapi.yml
- filename: bugbug-io-step-runs-api-openapi.yml
  format: yaml
  label: BugBug Step runs API
  slug: bugbug-io-step-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-step-runs-api-openapi.yml
- filename: bugbug-io-steps-api-openapi.yml
  format: yaml
  label: BugBug Steps API
  slug: bugbug-io-steps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-steps-api-openapi.yml
- filename: bugbug-io-suite-runs-api-openapi.yml
  format: yaml
  label: BugBug Suite runs API
  slug: bugbug-io-suite-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-suite-runs-api-openapi.yml
- filename: bugbug-io-suites-api-openapi.yml
  format: yaml
  label: BugBug Suites API
  slug: bugbug-io-suites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-suites-api-openapi.yml
- filename: bugbug-io-tags-api-openapi.yml
  format: yaml
  label: BugBug Tags API
  slug: bugbug-io-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-tags-api-openapi.yml
- filename: bugbug-io-test-runs-api-openapi.yml
  format: yaml
  label: BugBug Test runs API
  slug: bugbug-io-test-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-test-runs-api-openapi.yml
- filename: bugbug-io-tests-api-openapi.yml
  format: yaml
  label: BugBug Tests API
  slug: bugbug-io-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-tests-api-openapi.yml
- filename: bugbug-io-variables-api-openapi.yml
  format: yaml
  label: BugBug Variables API
  slug: bugbug-io-variables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-variables-api-openapi.yml
- filename: bugbug-io-visual-regression-api-openapi.yml
  format: yaml
  label: BugBug Visual regression API
  slug: bugbug-io-visual-regression-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugbug-io/openapi/bugbug-io-visual-regression-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bugbug.io
  spf: true
hosts:
- cert_expires: Jan 11 07:23:26 2027 GMT
  host: bugbug.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BugBug Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BugBug, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BugBug
provider_slug: bugbug-io
slug: bugbug-io-domain-security
source_filename: bugbug-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bugbug.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 07:23:26 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bugbug.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bugbug-io/security/bugbug-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Testing
- Automation
- Software-as-a-Service
- Low-Code
- No-Code
---
