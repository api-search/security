---
api_specs:
- filename: keda-metrics-api-openapi.yml
  format: yaml
  label: KEDA Metrics API
  slug: keda-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keda/refs/heads/main/openapi/keda-metrics-api-openapi.yml
- filename: keda-cloud-events-asyncapi.yml
  format: yaml
  label: KEDA CloudEventSource API
  slug: keda-cloud-event-source-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/keda/refs/heads/main/asyncapi/keda-cloud-events-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: keda.sh
  spf: false
hosts:
- cert_expires: Aug 13 05:54:42 2026 GMT
  host: keda.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KEDA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: KEDA
provider_slug: keda
slug: keda-domain-security
source_filename: keda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keda.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 05:54:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: keda.sh\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keda/refs/heads/main/security/keda-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Autoscaling
- CNCF
- Event-Driven
- Graduated
- Kubernetes
---
