---
api_specs:
- filename: silverflow-openapi.yml
  format: yaml
  label: Silverflow API
  slug: silverflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverflow/refs/heads/main/openapi/silverflow-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "visa.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: silverflow.com
  spf: true
hosts:
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: www.silverflow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: docs.silverflow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: eu-west-1.api.silverflow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Silverflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Silverflow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Silverflow
provider_slug: silverflow
slug: silverflow-domain-security
source_filename: silverflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.silverflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.silverflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: false\n- host: eu-west-1.api.silverflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: silverflow.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"visa.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silverflow/refs/heads/main/security/silverflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- Card Processing
- Acquiring
- Financial Services
- Tokenization
- 3-D Secure
- Disputes
- Chargebacks
- Interchange
- Reconciliation
- Point of Sale
- Netherlands
---
