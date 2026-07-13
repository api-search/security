---
api_specs:
- filename: kibana-openapi-original.yml
  format: yaml
  label: Kibana API
  slug: kibana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kibana/refs/heads/main/openapi/kibana-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elastic.co
  spf: true
hosts:
- cert_expires: Dec 12 21:06:03 2026 GMT
  host: www.elastic.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kibana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kibana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kibana
provider_slug: kibana
slug: kibana-domain-security
source_filename: kibana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elastic.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 21:06:03 2026 GMT\n  hsts: false\ndomains:\n- domain: elastic.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kibana/refs/heads/main/security/kibana-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Alerting
- Analytics
- Dashboards
- Elastic Stack
- Logging
- Monitoring
- Observability
- Visualization
---
