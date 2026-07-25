---
api_specs:
- filename: cim-openapi.html
  format: yaml
  label: Synopsys Coverity REST API
  slug: coverity
  spec_type: OpenAPI
  url: https://documentation.blackduck.com/bundle/coverity-docs/page/cim-api-docs/openapi/cim-openapi.html
- filename: synopsys-entitlements-api-openapi.yml
  format: yaml
  label: Synopsys Entitlements API
  slug: synopsys-entitlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synopsys/refs/heads/main/openapi/synopsys-entitlements-api-openapi.yml
- filename: synopsys-issues-api-openapi.yml
  format: yaml
  label: Synopsys Issues API
  slug: synopsys-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synopsys/refs/heads/main/openapi/synopsys-issues-api-openapi.yml
- filename: synopsys-licenses-api-openapi.yml
  format: yaml
  label: Synopsys Licenses API
  slug: synopsys-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synopsys/refs/heads/main/openapi/synopsys-licenses-api-openapi.yml
- filename: synopsys-projects-api-openapi.yml
  format: yaml
  label: Synopsys Projects API
  slug: synopsys-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synopsys/refs/heads/main/openapi/synopsys-projects-api-openapi.yml
- filename: synopsys-reports-api-openapi.yml
  format: yaml
  label: Synopsys Reports API
  slug: synopsys-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synopsys/refs/heads/main/openapi/synopsys-reports-api-openapi.yml
- filename: synopsys-scans-api-openapi.yml
  format: yaml
  label: Synopsys Scans API
  slug: synopsys-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synopsys/refs/heads/main/openapi/synopsys-scans-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: synopsys.com
  spf: true
hosts:
- cert_expires: Sep 16 21:31:06 2026 GMT
  host: www.synopsys.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: polaris.synopsys.com
  https: false
- host: community.synopsys.com
  https: false
kind: domain-security
layout: security
method: probed
name: Synopsys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synopsys, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Synopsys
provider_slug: synopsys
slug: synopsys-domain-security
source_filename: synopsys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.synopsys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 21:31:06 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: polaris.synopsys.com\n  https: false\n- host: community.synopsys.com\n  https: false\ndomains:\n- domain: synopsys.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synopsys/refs/heads/main/security/synopsys-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Software Security
- Application Security Testing
- Static Analysis
- Software Composition Analysis
- EDA Tools
- Semiconductor Design
- Fortune 1000
---
