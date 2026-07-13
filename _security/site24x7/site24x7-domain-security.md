---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Site24x7 REST API
  slug: site24x7-api
  spec_type: OpenAPI
  url: https://www.site24x7.com/help/api/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: site24x7.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: site24x7.eu
  spf: true
hosts:
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: www.site24x7.com
  hsts: true
  hsts_max_age: 64072000
  https: true
  tls_version: TLSv1.3
- host: api.site24x7.com
  https: false
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: www.site24x7.eu
  hsts: true
  hsts_max_age: 64072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Site24X7 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Site24x7, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Site24x7
provider_slug: site24x7
slug: site24x7-domain-security
source_filename: site24x7-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.site24x7.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 64072000\n- host: api.site24x7.com\n  https: false\n- host: www.site24x7.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 64072000\ndomains:\n- domain: site24x7.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: site24x7.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/site24x7/refs/heads/main/security/site24x7-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- Observability
- Uptime
- Infrastructure
- Cloud
- APM
- SLA
- Alerts
- Synthetic Monitoring
- Real User Monitoring
- Network Monitoring
- Server Monitoring
- Website Monitoring
- On-Call
- Status Pages
---
