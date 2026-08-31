---
api_specs:
- filename: resultid-endpoints-api-openapi.yml
  format: yaml
  label: Resultid Endpoints API
  slug: resultid-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resultid/refs/heads/main/openapi/resultid-endpoints-api-openapi.yml
- filename: resultid-insight-endpoints-api-openapi.yml
  format: yaml
  label: Resultid Insight endpoints API
  slug: resultid-insight-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resultid/refs/heads/main/openapi/resultid-insight-endpoints-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: resultid.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: resultid.com
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: www.resultid.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: docs.resultid.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Resultid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resultid, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Resultid
provider_slug: resultid
slug: resultid-domain-security
source_filename: resultid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.resultid.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\n- host: docs.resultid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: resultid.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: resultid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resultid/refs/heads/main/security/resultid-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Operational Intelligence
- Analytics
- Enterprise Software
- Artificial Intelligence
- Customer Experience
- Data Integration
- Revenue Intelligence
---
