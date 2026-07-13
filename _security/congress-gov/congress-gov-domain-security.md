---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Congress.gov API v3
  slug: congressgov-api-v3
  spec_type: OpenAPI
  url: https://api.congress.gov/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: congress.gov
  spf: true
hosts:
- cert_expires: Aug 18 21:44:05 2026 GMT
  host: www.congress.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 11:20:55 2026 GMT
  host: api.congress.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Congress Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Congress.gov API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Congress.gov API
provider_slug: congress-gov
slug: congress-gov-domain-security
source_filename: congress-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.congress.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 21:44:05 2026 GMT\n  hsts: null\n- host: api.congress.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 11:20:55 2026 GMT\n  hsts: null\ndomains:\n- domain: congress.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/congress-gov/refs/heads/main/security/congress-gov-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Government
- Legislative
- Congress
- Bills
- Amendments
- Members
- Treaties
- Nominations
- Congressional Record
- US Federal
---
