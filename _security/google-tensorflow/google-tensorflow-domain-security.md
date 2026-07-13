---
api_specs:
- filename: tensorflow-serving-openapi.yml
  format: yaml
  label: TensorFlow Serving REST API
  slug: tensorflow-serving-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-tensorflow/refs/heads/main/openapi/tensorflow-serving-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tensorflow.org
  spf: false
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tfhub.dev
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: www.tensorflow.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 14:16:37 2026 GMT
  host: tfhub.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Tensorflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google TensorFlow, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Google TensorFlow
provider_slug: google-tensorflow
slug: google-tensorflow-domain-security
source_filename: google-tensorflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tensorflow.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: tfhub.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 14:16:37 2026 GMT\n  hsts: null\ndomains:\n- domain: tensorflow.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: tfhub.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-tensorflow/refs/heads/main/security/google-tensorflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Deep Learning
- Google
- Machine Learning
- Model Serving
- Open Source
---
