---
api_specs:
- filename: checkmarx-applications-api-openapi.yml
  format: yaml
  label: Checkmarx Applications API
  slug: checkmarx-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-applications-api-openapi.yml
- filename: checkmarx-authentication-api-openapi.yml
  format: yaml
  label: Checkmarx Authentication API
  slug: checkmarx-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-authentication-api-openapi.yml
- filename: checkmarx-configuration-api-openapi.yml
  format: yaml
  label: Checkmarx Configuration API
  slug: checkmarx-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-configuration-api-openapi.yml
- filename: checkmarx-engines-api-openapi.yml
  format: yaml
  label: Checkmarx Engines API
  slug: checkmarx-engines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-engines-api-openapi.yml
- filename: checkmarx-groups-api-openapi.yml
  format: yaml
  label: Checkmarx Groups API
  slug: checkmarx-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-groups-api-openapi.yml
- filename: checkmarx-packages-api-openapi.yml
  format: yaml
  label: Checkmarx Packages API
  slug: checkmarx-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-packages-api-openapi.yml
- filename: checkmarx-presets-api-openapi.yml
  format: yaml
  label: Checkmarx Presets API
  slug: checkmarx-presets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-presets-api-openapi.yml
- filename: checkmarx-projects-api-openapi.yml
  format: yaml
  label: Checkmarx Projects API
  slug: checkmarx-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-projects-api-openapi.yml
- filename: checkmarx-queries-api-openapi.yml
  format: yaml
  label: Checkmarx Queries API
  slug: checkmarx-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-queries-api-openapi.yml
- filename: checkmarx-reports-api-openapi.yml
  format: yaml
  label: Checkmarx Reports API
  slug: checkmarx-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-reports-api-openapi.yml
- filename: checkmarx-results-api-openapi.yml
  format: yaml
  label: Checkmarx Results API
  slug: checkmarx-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-results-api-openapi.yml
- filename: checkmarx-risk-reports-api-openapi.yml
  format: yaml
  label: Checkmarx Risk Reports API
  slug: checkmarx-risk-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-risk-reports-api-openapi.yml
- filename: checkmarx-scans-api-openapi.yml
  format: yaml
  label: Checkmarx Scans API
  slug: checkmarx-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-scans-api-openapi.yml
- filename: checkmarx-settings-api-openapi.yml
  format: yaml
  label: Checkmarx Settings API
  slug: checkmarx-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-settings-api-openapi.yml
- filename: checkmarx-teams-api-openapi.yml
  format: yaml
  label: Checkmarx Teams API
  slug: checkmarx-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-teams-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: checkmarx.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: your-checkmarx-instance.com
  spf: false
hosts:
- cert_expires: Sep 17 16:25:35 2026 GMT
  host: www.checkmarx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 11:28:19 2026 GMT
  host: checkmarx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: your-checkmarx-instance.com
  https: false
kind: domain-security
layout: security
method: probed
name: Checkmarx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Checkmarx, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Checkmarx
provider_slug: checkmarx
slug: checkmarx-domain-security
source_filename: checkmarx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.checkmarx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:25:35 2026 GMT\n  hsts: false\n- host: checkmarx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 11:28:19 2026 GMT\n  hsts: false\n- host: your-checkmarx-instance.com\n  https: false\ndomains:\n- domain: checkmarx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: your-checkmarx-instance.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/security/checkmarx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Application Security
- Code Analysis
- DevSecOps
- SAST
- Security Testing
- Vulnerability Scanning
---
