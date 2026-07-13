---
api_specs:
- filename: openapi.json
  format: json
  label: Open States API v3
  slug: openstates-api-v3
  spec_type: OpenAPI
  url: https://v3.openstates.org/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pluralpolicy.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openstates.org
  spf: true
hosts:
- cert_expires: Sep 20 01:34:40 2026 GMT
  host: pluralpolicy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 17:45:48 2026 GMT
  host: docs.openstates.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: v3.openstates.org
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Openstates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open States, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open States
provider_slug: openstates
slug: openstates-domain-security
source_filename: openstates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pluralpolicy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:34:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.openstates.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:45:48 2026 GMT\n  hsts: false\n- host: v3.openstates.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: pluralpolicy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: openstates.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openstates/refs/heads/main/security/openstates-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Legislative Data
- Civic Technology
- State Legislature
- Bills
- Legislators
- Committees
- Open Data
- REST
- GraphQL
---
