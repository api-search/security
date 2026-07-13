---
api_specs:
- filename: flowable-bpmn-openapi.yml
  format: yaml
  label: Flowable BPMN API
  slug: flowable-bpmn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-bpmn-openapi.yml
- filename: flowable-cmmn-openapi.yml
  format: yaml
  label: Flowable CMMN API
  slug: flowable-cmmn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-cmmn-openapi.yml
- filename: flowable-dmn-openapi.yml
  format: yaml
  label: Flowable DMN API
  slug: flowable-dmn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-dmn-openapi.yml
- filename: flowable-form-openapi.yml
  format: yaml
  label: Flowable Form API
  slug: flowable-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-form-openapi.yml
- filename: flowable-content-openapi.yml
  format: yaml
  label: Flowable Content API
  slug: flowable-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-content-openapi.yml
- filename: flowable-idm-openapi.yml
  format: yaml
  label: Flowable IDM API
  slug: flowable-idm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-idm-openapi.yml
- filename: flowable-external-worker-openapi.yml
  format: yaml
  label: Flowable External Worker API
  slug: flowable-external-worker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/openapi/flowable-external-worker-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:sysadmin@flowable.com"
  - 0 issue "swisssign.com"
  - 0 issuewild "swisssign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flowable.com
  spf: true
hosts:
- cert_expires: Sep 13 04:44:47 2026 GMT
  host: www.flowable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  2 23:59:59 2026 GMT
  host: documentation.flowable.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flowable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flowable, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flowable
provider_slug: flowable
slug: flowable-domain-security
source_filename: flowable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flowable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:44:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documentation.flowable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: flowable.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:sysadmin@flowable.com\"\n  - 0 issue \"swisssign.com\"\n  - 0 issuewild \"swisssign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowable/refs/heads/main/security/flowable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- BPM
- Business Process Management
- Workflow
- BPMN
- CMMN
- DMN
- Process Automation
- Case Management
- Open Source
- REST API
---
