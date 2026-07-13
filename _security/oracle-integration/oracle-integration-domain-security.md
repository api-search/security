---
api_specs:
- filename: oracle-integration-developer-api.yaml
  format: yaml
  label: Oracle Integration Developer API
  slug: oracle-integration-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/openapi/oracle-integration-developer-api.yaml
- filename: oracle-integration-process-automation-api.yaml
  format: yaml
  label: Oracle Integration Process Automation API
  slug: oracle-integration-process-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/openapi/oracle-integration-process-automation-api.yaml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: cloud.oracle.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.oracle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oracle Integration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Integration, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle Integration
provider_slug: oracle-integration
slug: oracle-integration-domain-security
source_filename: oracle-integration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/security/oracle-integration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Management
- Automation
- B2B Integration
- Cloud Integration
- Enterprise Integration
- Integration
- iPaaS
- Process Automation
---
