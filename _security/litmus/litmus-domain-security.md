---
api_specs:
- filename: litmus-analytics-api-openapi.yml
  format: yaml
  label: Litmus Analytics API
  slug: litmus-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/openapi/litmus-analytics-api-openapi.yml
- filename: litmus-campaigns-api-openapi.yml
  format: yaml
  label: Litmus Campaigns API
  slug: litmus-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/openapi/litmus-campaigns-api-openapi.yml
- filename: litmus-clients-api-openapi.yml
  format: yaml
  label: Litmus Clients API
  slug: litmus-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/openapi/litmus-clients-api-openapi.yml
- filename: litmus-previews-api-openapi.yml
  format: yaml
  label: Litmus Previews API
  slug: litmus-previews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/openapi/litmus-previews-api-openapi.yml
- filename: litmus-results-api-openapi.yml
  format: yaml
  label: Litmus Results API
  slug: litmus-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/openapi/litmus-results-api-openapi.yml
- filename: litmus-tests-api-openapi.yml
  format: yaml
  label: Litmus Tests API
  slug: litmus-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/openapi/litmus-tests-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: litmus.com
  spf: true
hosts:
- cert_expires: Oct  1 08:46:54 2026 GMT
  host: www.litmus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 13:56:16 2026 GMT
  host: docs.litmus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: instant-api.litmus.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Litmus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Litmus, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Litmus
provider_slug: litmus
slug: litmus-domain-security
source_filename: litmus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.litmus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:46:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.litmus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 13:56:16 2026 GMT\n  hsts: false\n- host: instant-api.litmus.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: litmus.com\n  dnssec: false\n  caa:\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/security/litmus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Email Testing
- Marketing Tools
- Quality Assurance
---
