---
api_specs:
- filename: calyptia-cloud-openapi-original.yml
  format: yaml
  label: Calyptia Cloud API
  slug: calyptia-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calyptia/refs/heads/main/openapi/calyptia-cloud-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: calyptia.com
  spf: true
hosts:
- cert_expires: Aug 23 19:16:52 2026 GMT
  host: calyptia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 17:15:25 2026 GMT
  host: cloud-api.calyptia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 12:13:02 2026 GMT
  host: cloud-api-dev.calyptia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Calyptia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calyptia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Calyptia
provider_slug: calyptia
slug: calyptia-domain-security
source_filename: calyptia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calyptia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 19:16:52 2026 GMT\n  hsts: false\n- host: cloud-api.calyptia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:15:25 2026 GMT\n  hsts: null\n- host: cloud-api-dev.calyptia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 12:13:02 2026 GMT\n  hsts: null\ndomains:\n- domain: calyptia.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calyptia/refs/heads/main/security/calyptia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Infrastructure
- Observability
- Telemetry
- Logging
- Fluent Bit
- Data Pipeline
- Kubernetes
- DevOps
---
