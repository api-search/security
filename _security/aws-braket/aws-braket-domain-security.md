---
api_specs:
- filename: aws-braket-quantum-tasks-api-openapi.yml
  format: yaml
  label: AWS Braket Quantum Tasks API
  slug: aws-braket-quantum-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/openapi/aws-braket-quantum-tasks-api-openapi.yml
- filename: aws-braket-devices-api-openapi.yml
  format: yaml
  label: AWS Braket Devices API
  slug: aws-braket-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/openapi/aws-braket-devices-api-openapi.yml
- filename: aws-braket-hybrid-jobs-api-openapi.yml
  format: yaml
  label: AWS Braket Hybrid Jobs API
  slug: aws-braket-hybrid-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/openapi/aws-braket-hybrid-jobs-api-openapi.yml
- filename: aws-braket-spending-limits-api-openapi.yml
  format: yaml
  label: AWS Braket Spending Limits API
  slug: aws-braket-spending-limits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/openapi/aws-braket-spending-limits-api-openapi.yml
- filename: aws-braket-tags-api-openapi.yml
  format: yaml
  label: AWS Braket Tags API
  slug: aws-braket-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/openapi/aws-braket-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: braket.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aws Braket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AWS Braket, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AWS Braket
provider_slug: aws-braket
slug: aws-braket-domain-security
source_filename: aws-braket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: braket.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-braket/refs/heads/main/security/aws-braket-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Quantum Computing
- QPU
- Simulator
- Hybrid Jobs
- OpenQASM
- PennyLane
- Qiskit
- Quantum
---
