---
api_specs:
- filename: openobserve-openapi.json
  format: json
  label: OpenObserve
  slug: openobserve
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openobserve/refs/heads/main/openapi/openobserve-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: openobserve.ai
  spf: true
hosts:
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: openobserve.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 17:48:50 2026 GMT
  host: api.openobserve.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openobserve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenObserve, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: OpenObserve
provider_slug: openobserve
slug: openobserve-domain-security
source_filename: openobserve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openobserve.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openobserve.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:48:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openobserve.ai\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openobserve/refs/heads/main/security/openobserve-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Observability
- Logs
- Metrics
- Traces
- RUM
- Open Source
---
