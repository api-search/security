---
api_specs:
- filename: scale-computing-fleet-manager-openapi.json
  format: json
  label: SC//Fleet Manager API
  slug: scfleet-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-fleet-manager-openapi.json
- filename: scale-computing-core-openapi.json
  format: json
  label: Scale Computing Platform Core API
  slug: scale-computing-platform-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-core-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scalecomputing.com
  spf: true
hosts:
- cert_expires: Oct 18 08:13:39 2026 GMT
  host: www.scalecomputing.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 21:07:17 2026 GMT
  host: api.scalecomputing.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scale Computing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scale Computing, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scale Computing
provider_slug: scale-computing
slug: scale-computing-domain-security
source_filename: scale-computing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scalecomputing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 08:13:39 2026 GMT\n  hsts: false\n- host: api.scalecomputing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 21:07:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scalecomputing.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/security/scale-computing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Edge Computing
- Hyperconverged Infrastructure
- Virtualization
- Infrastructure Management
- Fleet Management
- Virtual Machines
- Observability
- Infrastructure as Code
- Kubernetes
- Company
---
