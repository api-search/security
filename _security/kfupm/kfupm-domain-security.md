---
api_specs:
- filename: oai2
  format: yaml
  label: KFUPM ePrints OAI-PMH
  slug: eprints-oai
  spec_type: OpenAPI
  url: https://eprints.kfupm.edu.sa/cgi/oai2?verb=Identify
- filename: kfupm-pure-ws.yaml
  format: yaml
  label: KFUPM Pure Web Services API
  slug: pure-ws
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/openapi/kfupm-pure-ws.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kfupm.edu.sa
  spf: true
hosts:
- cert_expires: Feb  5 08:41:04 2027 GMT
  host: www.kfupm.edu.sa
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 08:41:04 2027 GMT
  host: eprints.kfupm.edu.sa
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 01:02:33 2026 GMT
  host: pure.kfupm.edu.sa
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kfupm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for King Fahd University of Petroleum & Minerals, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: King Fahd University of Petroleum & Minerals
provider_slug: kfupm
slug: kfupm-domain-security
source_filename: kfupm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kfupm.edu.sa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 08:41:04 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eprints.kfupm.edu.sa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 08:41:04 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: pure.kfupm.edu.sa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 01:02:33 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: kfupm.edu.sa\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/security/kfupm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Repository
- Saudi Arabia
- Middle East
---
