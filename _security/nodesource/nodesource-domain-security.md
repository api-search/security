---
api_specs:
- filename: nodesource-openapi-generated.yml
  format: yaml
  label: NodeSource API
  slug: nodesource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nodesource/openapi/_ae-authored/nodesource-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nodesource.com
  spf: true
hosts:
- cert_expires: Apr 23 23:59:59 2027 GMT
  host: www.nodesource.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nodesource Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NodeSource, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NodeSource
provider_slug: nodesource
slug: nodesource-domain-security
source_filename: nodesource-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nodesource.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 23 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nodesource.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/nodesource/security/nodesource-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Node.js
- Enterprise
- Monitoring
- Security
- Performance
---
