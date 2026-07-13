---
api_specs:
- filename: openapi.yml
  format: yaml
  label: BigML REST API
  slug: bigml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bigml.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: bigml.io
  spf: false
hosts:
- cert_expires: Oct  4 22:11:30 2026 GMT
  host: bigml.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 22:39:15 2026 GMT
  host: bigml.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bigml Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BigML, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BigML
provider_slug: bigml
slug: bigml-domain-security
source_filename: bigml-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bigml.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:11:30 2026 GMT\n  hsts: false\n- host: bigml.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:39:15 2026 GMT\n  hsts: null\ndomains:\n- domain: bigml.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bigml.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/security/bigml-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Machine Learning
- Artificial Intelligence
- Predictions
- Datasets
- Models
- Clustering
- Anomaly Detection
- Time Series
- Deep Learning
---
