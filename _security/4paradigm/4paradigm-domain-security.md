---
api_specs:
- filename: 4paradigm-account-api-openapi.yml
  format: yaml
  label: 4Paradigm Account API
  slug: 4paradigm-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-account-api-openapi.yml
- filename: 4paradigm-applications-api-openapi.yml
  format: yaml
  label: 4Paradigm Applications API
  slug: 4paradigm-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-applications-api-openapi.yml
- filename: 4paradigm-competition-api-openapi.yml
  format: yaml
  label: 4Paradigm Competition API
  slug: 4paradigm-competition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-competition-api-openapi.yml
- filename: 4paradigm-computeunit-api-openapi.yml
  format: yaml
  label: 4Paradigm Computeunit API
  slug: 4paradigm-computeunit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-computeunit-api-openapi.yml
- filename: 4paradigm-computing-resource-api-openapi.yml
  format: yaml
  label: 4Paradigm Computing Resource API
  slug: 4paradigm-computing-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-computing-resource-api-openapi.yml
- filename: 4paradigm-environments-api-openapi.yml
  format: yaml
  label: 4Paradigm Environments API
  slug: 4paradigm-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-environments-api-openapi.yml
- filename: 4paradigm-finished-api-openapi.yml
  format: yaml
  label: 4Paradigm Finished API
  slug: 4paradigm-finished-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-finished-api-openapi.yml
- filename: 4paradigm-images-api-openapi.yml
  format: yaml
  label: 4Paradigm Images API
  slug: 4paradigm-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-images-api-openapi.yml
- filename: 4paradigm-logs-api-openapi.yml
  format: yaml
  label: 4Paradigm Logs API
  slug: 4paradigm-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-logs-api-openapi.yml
- filename: 4paradigm-releases-api-openapi.yml
  format: yaml
  label: 4Paradigm Releases API
  slug: 4paradigm-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-releases-api-openapi.yml
- filename: 4paradigm-storage-api-openapi.yml
  format: yaml
  label: 4Paradigm Storage API
  slug: 4paradigm-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-storage-api-openapi.yml
- filename: 4paradigm-users-api-openapi.yml
  format: yaml
  label: 4Paradigm Users API
  slug: 4paradigm-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-users-api-openapi.yml
- filename: 4paradigm-app-store-api-openapi.yml
  format: yaml
  label: 4Paradigm App Store API
  slug: 4paradigm-app-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-app-store-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 4paradigm.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: openmldb.ai
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: www.4paradigm.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: openmldb.ai
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
- host: 127.0.0.1
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: 4Paradigm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4Paradigm, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 4Paradigm
provider_slug: 4paradigm
slug: 4paradigm-domain-security
source_filename: 4paradigm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.4paradigm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\n- host: openmldb.ai\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: 4paradigm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: openmldb.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/security/4paradigm-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Feature Store
- Database
- Open Source
- MLOps
- Agents
- Robotics
- Kubernetes
---
