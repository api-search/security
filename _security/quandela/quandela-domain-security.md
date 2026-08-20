---
api_specs:
- filename: quandela-perceval-job-openapi.yml
  format: yaml
  label: Quandela Cloud API
  slug: quandela-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandela/refs/heads/main/openapi/quandela-perceval-job-openapi.yml
- filename: quandela-quantum-toolbox-openapi.yml
  format: yaml
  label: Quandela Quantum Toolbox API
  slug: quandela-quantum-toolbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandela/refs/heads/main/openapi/quandela-quantum-toolbox-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quandela.com
  spf: true
hosts:
- cert_expires: Nov  4 12:57:55 2026 GMT
  host: www.quandela.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 22:09:50 2026 GMT
  host: api.cloud.quandela.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quandela Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quandela, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quandela
provider_slug: quandela
slug: quandela-domain-security
source_filename: quandela-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quandela.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 12:57:55 2026 GMT\n  hsts: false\n- host: api.cloud.quandela.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 22:09:50 2026 GMT\n  hsts: false\ndomains:\n- domain: quandela.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quandela/refs/heads/main/security/quandela-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Quantum Computing
- Photonic Quantum
- Photonics
- Single Photon Sources
- Quantum Hardware
- Quantum Cloud
- QPU
- Perceval
- Python SDK
- Quantum Random Number Generation
- Quantum Simulation
- Variational Quantum Algorithms
- Quantum Chemistry
- Graph Algorithms
- Job Orchestration
- Open-Source
- France
---
