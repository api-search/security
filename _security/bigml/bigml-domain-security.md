---
api_specs:
- filename: bigml-anomaly-detection-api-openapi.yml
  format: yaml
  label: BigML Anomaly Detection API
  slug: bigml-anomaly-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-anomaly-detection-api-openapi.yml
- filename: bigml-batch-operations-api-openapi.yml
  format: yaml
  label: BigML Batch Operations API
  slug: bigml-batch-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-batch-operations-api-openapi.yml
- filename: bigml-clustering-api-openapi.yml
  format: yaml
  label: BigML Clustering API
  slug: bigml-clustering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-clustering-api-openapi.yml
- filename: bigml-data-connectors-api-openapi.yml
  format: yaml
  label: BigML Data Connectors API
  slug: bigml-data-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-data-connectors-api-openapi.yml
- filename: bigml-datasets-api-openapi.yml
  format: yaml
  label: BigML Datasets API
  slug: bigml-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-datasets-api-openapi.yml
- filename: bigml-ensembles-api-openapi.yml
  format: yaml
  label: BigML Ensembles API
  slug: bigml-ensembles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-ensembles-api-openapi.yml
- filename: bigml-evaluations-api-openapi.yml
  format: yaml
  label: BigML Evaluations API
  slug: bigml-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-evaluations-api-openapi.yml
- filename: bigml-models-api-openapi.yml
  format: yaml
  label: BigML Models API
  slug: bigml-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-models-api-openapi.yml
- filename: bigml-predictions-api-openapi.yml
  format: yaml
  label: BigML Predictions API
  slug: bigml-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-predictions-api-openapi.yml
- filename: bigml-projects-api-openapi.yml
  format: yaml
  label: BigML Projects API
  slug: bigml-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-projects-api-openapi.yml
- filename: bigml-sources-api-openapi.yml
  format: yaml
  label: BigML Sources API
  slug: bigml-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-sources-api-openapi.yml
- filename: bigml-supervised-learning-api-openapi.yml
  format: yaml
  label: BigML Supervised Learning API
  slug: bigml-supervised-learning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-supervised-learning-api-openapi.yml
- filename: bigml-time-series-api-openapi.yml
  format: yaml
  label: BigML Time Series API
  slug: bigml-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-time-series-api-openapi.yml
- filename: bigml-unsupervised-learning-api-openapi.yml
  format: yaml
  label: BigML Unsupervised Learning API
  slug: bigml-unsupervised-learning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-unsupervised-learning-api-openapi.yml
- filename: bigml-whizzml-scripting-api-openapi.yml
  format: yaml
  label: BigML WhizzML Scripting API
  slug: bigml-whizzml-scripting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigml/refs/heads/main/openapi/bigml-whizzml-scripting-api-openapi.yml
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
- Machine-Learning
- Artificial Intelligence
- Predictions
- Datasets
- Models
- Clustering
- Anomaly Detection
- Time Series
- Deep Learning
---
