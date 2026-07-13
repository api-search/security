---
api_specs:
- filename: acadia-platform.yaml
  format: yaml
  label: Acadia Platform API
  slug: acadia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/openapi/acadia-platform.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acadia-software.com
  spf: true
hosts:
- cert_expires: Aug  7 22:30:06 2026 GMT
  host: www.acadia-software.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.acadia-software.com
  https: false
kind: domain-security
layout: security
method: probed
name: Acadia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acadia, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acadia
provider_slug: acadia
slug: acadia-domain-security
source_filename: acadia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acadia-software.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 22:30:06 2026 GMT\n  hsts: false\n- host: api.acadia-software.com\n  https: false\ndomains:\n- domain: acadia-software.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/security/acadia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Connected Worker
- Knowledge Management
- Manufacturing
- Skills Management
- Training
- Workforce Development
---
