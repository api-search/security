---
api_specs:
- filename: graphite-connect-openapi-generated.yml
  format: yaml
  label: Graphite Connect API
  slug: graphite-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphite-connect/refs/heads/main/openapi/_ae-authored/graphite-connect-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: graphiteconnect.com
  spf: true
hosts:
- cert_expires: Nov 13 20:59:25 2026 GMT
  host: www.graphiteconnect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Graphite Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Graphite Connect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Graphite Connect
provider_slug: graphite-connect
slug: graphite-connect-domain-security
source_filename: graphite-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.graphiteconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 20:59:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: graphiteconnect.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphite-connect/refs/heads/main/security/graphite-connect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Supplier Management
- Procurement
- AI
- Risk Management
---
