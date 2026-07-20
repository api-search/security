---
api_specs:
- filename: catchpoint-rest-api-v2-openapi-original.json
  format: json
  label: Catchpoint REST API v2
  slug: catchpoint-rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/catchpoint/refs/heads/main/openapi/catchpoint-rest-api-v2-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: catchpoint.com
  spf: true
hosts:
- cert_expires: Sep 30 21:53:26 2026 GMT
  host: www.catchpoint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Catchpoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Catchpoint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Catchpoint
provider_slug: catchpoint
slug: catchpoint-domain-security
source_filename: catchpoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.catchpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:53:26 2026 GMT\n  hsts: false\ndomains:\n- domain: catchpoint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catchpoint/refs/heads/main/security/catchpoint-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Devops
- Monitoring
- Observability
- Internet Performance Monitoring
- Synthetic Monitoring
- Real User Monitoring
- Network Monitoring
- BGP Monitoring
- Digital Experience Monitoring
---
