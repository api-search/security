---
api_specs:
- filename: deepchecks-openapi.yml
  format: yaml
  label: Deepchecks LLM Interactions / Logging API
  slug: llm-interactions-logging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-openapi.yml
- filename: deepchecks-openapi.yml
  format: yaml
  label: Deepchecks Applications / Versions API
  slug: applications-versions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-openapi.yml
- filename: deepchecks-openapi.yml
  format: yaml
  label: Deepchecks Annotations API
  slug: annotations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-openapi.yml
- filename: deepchecks-openapi.yml
  format: yaml
  label: Deepchecks Properties API
  slug: properties
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deepchecks.com
  spf: true
hosts:
- cert_expires: Sep  6 18:05:11 2026 GMT
  host: www.deepchecks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 07:02:29 2026 GMT
  host: llmdocs.deepchecks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: app.llm.deepchecks.com
  https: false
kind: domain-security
layout: security
method: probed
name: Deepchecks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deepchecks, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Deepchecks
provider_slug: deepchecks
slug: deepchecks-domain-security
source_filename: deepchecks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deepchecks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:05:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: llmdocs.deepchecks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 07:02:29 2026 GMT\n  hsts: null\n- host: app.llm.deepchecks.com\n  https: false\ndomains:\n- domain: deepchecks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/security/deepchecks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Evaluation
- Testing
- Monitoring
---
