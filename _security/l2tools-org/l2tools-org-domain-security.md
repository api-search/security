---
api_specs:
- filename: l2tools-org-npcs-api-openapi.yml
  format: yaml
  label: L2Tools NPCs API
  slug: l2tools-org-npcs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/l2tools-org/openapi/l2tools-org-npcs-api-openapi.yml
- filename: l2tools-org-tools-api-openapi.yml
  format: yaml
  label: L2Tools Tools API
  slug: l2tools-org-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/l2tools-org/openapi/l2tools-org-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: l2tools.org
  spf: true
hosts:
- cert_expires: Jan 22 13:37:18 2027 GMT
  host: l2tools.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: L2Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for L2Tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: L2Tools
provider_slug: l2tools-org
slug: l2tools-org-domain-security
source_filename: l2tools-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: l2tools.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 13:37:18 2027 GMT\n  hsts: false\ndomains:\n- domain: l2tools.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/l2tools-org/security/l2tools-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Gaming
- Database
- Tools
- Community
- Lineage2
---
