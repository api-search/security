---
api_specs:
- filename: soda-health-docs-portal-openapi-original.json
  format: json
  label: Evermore Docs Portal API
  slug: evermore-docs-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soda-health/refs/heads/main/openapi/soda-health-docs-portal-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: evermoreoutcomes.com
  spf: true
hosts:
- cert_expires: Sep 27 20:38:36 2026 GMT
  host: docs.evermoreoutcomes.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soda Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soda Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Soda Health
provider_slug: soda-health
slug: soda-health-domain-security
source_filename: soda-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.evermoreoutcomes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 20:38:36 2026 GMT\n  hsts: null\ndomains:\n- domain: evermoreoutcomes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soda-health/refs/heads/main/security/soda-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Health Benefits
- Medicare Advantage
- Medicaid
- Supplemental Benefits
- Benefits Administration
- Documentation Portal
---
