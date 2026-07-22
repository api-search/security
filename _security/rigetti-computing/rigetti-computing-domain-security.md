---
api_specs:
- filename: rigetti-computing-qcs-openapi-original.yml
  format: yaml
  label: Rigetti QCS API
  slug: rigetti-qcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rigetti-computing/refs/heads/main/openapi/rigetti-computing-qcs-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rigetti.com
  spf: true
hosts:
- cert_expires: Oct  6 06:32:00 2026 GMT
  host: www.rigetti.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: docs.rigetti.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: api.qcs.rigetti.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rigetti Computing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rigetti Computing, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rigetti Computing
provider_slug: rigetti-computing
slug: rigetti-computing-domain-security
source_filename: rigetti-computing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rigetti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 06:32:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.rigetti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: false\n- host: api.qcs.rigetti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: rigetti.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rigetti-computing/refs/heads/main/security/rigetti-computing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Quantum Computing
- Quantum Cloud
- Developer Tools
- SDKs
- Superconducting Qubits
- Scientific Computing
- Deep Tech
---
