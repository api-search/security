---
api_specs:
- filename: director-of-national-intelligence-wp-content-openapi.yml
  format: yaml
  label: ODNI Public Content API
  slug: odni-public-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/director-of-national-intelligence/refs/heads/main/openapi/director-of-national-intelligence-wp-content-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: odni.gov
  spf: true
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: www.odni.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Director Of National Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Director of National Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Director of National Intelligence
provider_slug: director-of-national-intelligence
slug: director-of-national-intelligence-domain-security
source_filename: director-of-national-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.odni.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: odni.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/director-of-national-intelligence/refs/heads/main/security/director-of-national-intelligence-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal-Government
- Intelligence
- National-Security
- Government
- Public-Sector
- Transparency
- News
- Publications
---
