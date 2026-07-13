---
api_specs:
- filename: tensorflow-serving-openapi.yml
  format: yaml
  label: TensorFlow Serving REST API
  slug: tensorflow-serving-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensorflow/refs/heads/main/openapi/tensorflow-serving-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tensorflow.org
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: jsdelivr.net
  spf: false
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: www.tensorflow.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 01:11:06 2026 GMT
  host: js.tensorflow.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: cdn.jsdelivr.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tensorflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TensorFlow, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TensorFlow
provider_slug: tensorflow
slug: tensorflow-domain-security
source_filename: tensorflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tensorflow.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: js.tensorflow.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 01:11:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cdn.jsdelivr.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tensorflow.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: jsdelivr.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tensorflow/refs/heads/main/security/tensorflow-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- Deep Learning
- JavaScript
- Machine Learning
- Model Serving
- Neural Networks
- Open Source
- Python
---
