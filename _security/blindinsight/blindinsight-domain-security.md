---
api_specs:
- filename: blindinsight-openapi-original.yml
  format: yaml
  label: Blind Insight REST API
  slug: blind-insight-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/openapi/blindinsight-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blindinsight.io
  spf: true
hosts:
- host: blindinsight.io
  https: false
- cert_expires: Sep  2 03:53:19 2026 GMT
  host: docs.blindinsight.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 15:21:10 2026 GMT
  host: api.app.blindinsight.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blindinsight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlindInsight, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BlindInsight
provider_slug: blindinsight
slug: blindinsight-domain-security
source_filename: blindinsight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blindinsight.io\n  https: false\n- host: docs.blindinsight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 03:53:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.app.blindinsight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:21:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blindinsight.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blindinsight/refs/heads/main/security/blindinsight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Encryption
- Privacy
- Confidential Computing
- Data
- Machine Learning
- Compliance
- Cryptography
---
