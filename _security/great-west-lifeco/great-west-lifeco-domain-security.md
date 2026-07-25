---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: greatwestlifeco.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: empower.com
  spf: true
- caa: []
  dmarc: true
  dmarc_note: _dmarc.canadalife.com CNAMEs to _dmarc.reject.canadalife.com; policy v=DMARC1; p=reject with Proofpoint rua/ruf reporting.
  dmarc_policy: reject
  dnssec: false
  domain: canadalife.com
  spf: true
hosts:
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: www.greatwestlifeco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 09:47:12 2026 GMT
  host: developer.empower.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 06:21:50 2026 GMT
  host: api.empower.com
  hsts: null
  https: true
  note: AWS API Gateway. Every anonymous request returns {"message":"Forbidden"}, so no HSTS header is observable.
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: www.canadalife.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: api.canadalife.com
  hsts: null
  https: true
  note: Apigee behind a Google Cloud load balancer. Anonymous requests to undocumented paths return HTTP 403 at the edge, so no HSTS header is observable; /.well-known/openid-configuration and /oauth2/v1/jwks do answer 200.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Great West Lifeco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Great-West Lifeco, probed live across 5 host(s) and 3 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Great-West Lifeco
provider_slug: great-west-lifeco
slug: great-west-lifeco-domain-security
source_filename: great-west-lifeco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.greatwestlifeco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.empower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 09:47:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.empower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 06:21:50 2026 GMT\n  hsts: null\n  note: >-\n    AWS API Gateway. Every anonymous request returns {\"message\":\"Forbidden\"},\n    so no HSTS header is observable.\n- host: www.canadalife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: api.canadalife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: null\n  note: >-\n\
  \    Apigee behind a Google Cloud load balancer. Anonymous requests to\n    undocumented paths return HTTP 403 at the edge, so no HSTS header is\n    observable; /.well-known/openid-configuration and /oauth2/v1/jwks do\n    answer 200.\ndomains:\n- domain: greatwestlifeco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: empower.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: canadalife.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_note: >-\n    _dmarc.canadalife.com CNAMEs to _dmarc.reject.canadalife.com; policy\n    v=DMARC1; p=reject with Proofpoint rua/ruf reporting.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/great-west-lifeco/refs/heads/main/security/great-west-lifeco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Canada
- Life Insurance
- Health Insurance
- Employee Benefits
- Retirement
- Wealth Management
- Reinsurance
- Annuities
- Partner Gated
---
