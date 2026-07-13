---
api_specs:
- filename: d-wave-solvers-api-openapi.yml
  format: yaml
  label: D-Wave Solver API (SAPI) - Solvers
  slug: d-wave-solver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-solvers-api-openapi.yml
- filename: d-wave-problems-api-openapi.yml
  format: yaml
  label: D-Wave Solver API (SAPI) - Problems
  slug: d-wave-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-problems-api-openapi.yml
- filename: d-wave-metadata-api-openapi.yml
  format: yaml
  label: D-Wave Metadata API - Regions
  slug: d-wave-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-metadata-api-openapi.yml
- filename: d-wave-leap-account-api-openapi.yml
  format: yaml
  label: D-Wave Leap Account API
  slug: d-wave-leap-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-leap-account-api-openapi.yml
- filename: d-wave-hybrid-solvers-openapi.yml
  format: yaml
  label: D-Wave Leap Hybrid Solvers
  slug: d-wave-hybrid-solvers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-hybrid-solvers-openapi.yml
- filename: d-wave-qpu-samplers-openapi.yml
  format: yaml
  label: D-Wave QPU Samplers (Advantage / Advantage2)
  slug: d-wave-qpu-samplers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/openapi/d-wave-qpu-samplers-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dwavequantum.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:info@dwavesys.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dwavesys.com
  spf: true
hosts:
- cert_expires: Sep 23 02:43:13 2026 GMT
  host: www.dwavequantum.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 27 18:06:18 2026 GMT
  host: docs.dwavequantum.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: cloud.dwavesys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: D Wave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for D-Wave, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: D-Wave
provider_slug: d-wave
slug: d-wave-domain-security
source_filename: d-wave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dwavequantum.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 02:43:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.dwavequantum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 18:06:18 2026 GMT\n  hsts: false\n- host: cloud.dwavesys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dwavequantum.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dwavesys.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"comodoca.com\"\
  \n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:info@dwavesys.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d-wave/refs/heads/main/security/d-wave-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Quantum Computing
- Quantum Annealing
- Optimization
- Hybrid Quantum-Classical
- Ising
- QUBO
- Industrial Optimization
- Sampling
- Leap
- Ocean SDK
- SAPI
---
