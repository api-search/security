---
api_specs:
- filename: swarmia-openapi.yml
  format: yaml
  label: Swarmia Metrics Export API
  slug: metrics-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swarmia/refs/heads/main/openapi/swarmia-openapi.yml
- filename: swarmia-openapi.yml
  format: yaml
  label: Swarmia Deployments & Events Ingestion API
  slug: deployments-events-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swarmia/refs/heads/main/openapi/swarmia-openapi.yml
- filename: swarmia-openapi.yml
  format: yaml
  label: Swarmia Investment Categories API
  slug: investment-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swarmia/refs/heads/main/openapi/swarmia-openapi.yml
- filename: swarmia-openapi.yml
  format: yaml
  label: Swarmia Webhooks & Notifications API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swarmia/refs/heads/main/openapi/swarmia-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: swarmia.com
  spf: true
hosts:
- cert_expires: Sep 14 10:09:40 2026 GMT
  host: www.swarmia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 18:31:14 2026 GMT
  host: help.swarmia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 20:43:41 2026 GMT
  host: app.swarmia.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swarmia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swarmia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Swarmia
provider_slug: swarmia
slug: swarmia-domain-security
source_filename: swarmia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swarmia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 10:09:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.swarmia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:31:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.swarmia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:43:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: swarmia.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swarmia/refs/heads/main/security/swarmia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Engineering Effectiveness
- Developer Productivity
- DORA
- Software Delivery
- Analytics
---
