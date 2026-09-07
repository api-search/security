---
api_specs:
- filename: 4paradigm-openaios-platform.yaml
  format: yaml
  label: OpenAIOS Platform API (Pineapple)
  slug: 4paradigm-openaios-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-openaios-platform.yaml
- filename: 4paradigm-openaios-billing.yaml
  format: yaml
  label: OpenAIOS Platform Billing API
  slug: 4paradigm-openaios-billing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/4paradigm/refs/heads/main/openapi/4paradigm-openaios-billing.yaml
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
- Databases
- Open Source
- MLOps
- Agents
- Robotics
- Kubernetes
---
