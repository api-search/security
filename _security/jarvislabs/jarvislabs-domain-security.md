---
api_specs:
- filename: jarvislabs-openapi.yml
  format: yaml
  label: JarvisLabs Instances API
  slug: jarvislabs-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/openapi/jarvislabs-openapi.yml
- filename: jarvislabs-openapi.yml
  format: yaml
  label: JarvisLabs GPU Types API
  slug: jarvislabs-gpu-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/openapi/jarvislabs-openapi.yml
- filename: jarvislabs-openapi.yml
  format: yaml
  label: JarvisLabs Templates API
  slug: jarvislabs-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/openapi/jarvislabs-openapi.yml
- filename: jarvislabs-openapi.yml
  format: yaml
  label: JarvisLabs Inference & Deploy API
  slug: jarvislabs-inference-deploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/openapi/jarvislabs-openapi.yml
- filename: jarvislabs-openapi.yml
  format: yaml
  label: JarvisLabs SDK & CLI
  slug: jarvislabs-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/openapi/jarvislabs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jarvislabs.ai
  spf: true
hosts:
- cert_expires: Oct  1 22:34:04 2026 GMT
  host: jarvislabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 00:45:31 2026 GMT
  host: docs.jarvislabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.jarvislabs.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Jarvislabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JarvisLabs, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: JarvisLabs
provider_slug: jarvislabs
slug: jarvislabs-domain-security
source_filename: jarvislabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jarvislabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 22:34:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.jarvislabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:45:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.jarvislabs.ai\n  https: false\ndomains:\n- domain: jarvislabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jarvislabs/refs/heads/main/security/jarvislabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- GPU
- Cloud
- Infrastructure
- Compute
---
