---
api_specs:
- filename: ray-openapi.yml
  format: yaml
  label: Ray Jobs REST API
  slug: jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ray/refs/heads/main/openapi/ray-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ray.io
  spf: true
hosts:
- cert_expires: Oct  8 23:34:51 2026 GMT
  host: www.ray.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 20:01:26 2026 GMT
  host: docs.ray.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Ray Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ray, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ray
provider_slug: ray
slug: ray-domain-security
source_filename: ray-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ray.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:34:51 2026 GMT\n  hsts: false\n- host: docs.ray.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 20:01:26 2026 GMT\n  hsts: false\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: ray.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ray/refs/heads/main/security/ray-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Distributed Computing
- Machine Learning
- AI Infrastructure
- Python
- Model Serving
- Open Source
- Compute
---
