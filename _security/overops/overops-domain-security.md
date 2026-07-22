---
api_specs:
- filename: overops-openapi-original.json
  format: json
  label: OverOps REST API
  slug: overops-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: overops.com
  spf: true
hosts:
- cert_expires: Aug 10 23:59:59 2026 GMT
  host: api.overops.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Overops Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Overops, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Overops
provider_slug: overops
slug: overops-domain-security
source_filename: overops-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.overops.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: overops.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/security/overops-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Observability
- Reliability
- Error Monitoring
- Application Performance
- Java
- DevOps
- Code Quality
---
