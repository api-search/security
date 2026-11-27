---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: configo.org
  spf: true
hosts:
- cert_expires: Dec 27 17:01:12 2026 GMT
  host: configo.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Configo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Configo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Configo
provider_slug: configo-org
slug: configo-org-domain-security
source_filename: configo-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: configo.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 17:01:12 2026 GMT\n  hsts: false\ndomains:\n- domain: configo.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/configo-org/security/configo-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- CPQ
- Product Configurator
- Manufacturing
- Pricing
- CRM
- Inventory
- MCP
---
