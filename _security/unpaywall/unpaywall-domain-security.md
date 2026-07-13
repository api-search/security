---
api_specs:
- filename: unpaywall-openapi.yml
  format: yaml
  label: Unpaywall API
  slug: unpaywall
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unpaywall/refs/heads/main/openapi/unpaywall-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: unpaywall.org
  spf: false
hosts:
- cert_expires: Oct  5 00:31:09 2026 GMT
  host: unpaywall.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 23:51:13 2026 GMT
  host: api.unpaywall.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unpaywall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unpaywall, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Unpaywall
provider_slug: unpaywall
slug: unpaywall-domain-security
source_filename: unpaywall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unpaywall.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:31:09 2026 GMT\n  hsts: false\n- host: api.unpaywall.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:51:13 2026 GMT\n  hsts: false\ndomains:\n- domain: unpaywall.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unpaywall/refs/heads/main/security/unpaywall-domain-security.yml
summary_line: TLSv1.3
tags:
- Open Access
- Scholarly Articles
- Research
- Academic
- Libraries
- DOI
- Science
---
