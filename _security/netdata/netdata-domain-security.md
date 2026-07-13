---
api_specs:
- filename: netdata-swagger.yaml
  format: yaml
  label: Netdata Agent API
  slug: agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/netdata/netdata/master/src/web/api/netdata-swagger.yaml
- filename: netdata-cloud-api-openapi.yml
  format: yaml
  label: Netdata Cloud API
  slug: cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/openapi/netdata-cloud-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: netdata.cloud
  spf: true
hosts:
- cert_expires: Oct  2 19:18:18 2026 GMT
  host: www.netdata.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 05:07:14 2026 GMT
  host: learn.netdata.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 18:05:47 2026 GMT
  host: app.netdata.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netdata, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Netdata
provider_slug: netdata
slug: netdata-domain-security
source_filename: netdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.netdata.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:18:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.netdata.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 05:07:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.netdata.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 18:05:47 2026 GMT\n  hsts: false\ndomains:\n- domain: netdata.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netdata/refs/heads/main/security/netdata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Monitoring
- Observability
- Infrastructure
- Metrics
- Alerts
- Real-Time
- APM
- DevOps
---
