---
api_specs:
- filename: obligationsign-com-openapi-generated.yml
  format: yaml
  label: obligationsign-com API
  slug: obligationsign-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obligationsign-com/openapi/_ae-authored/obligationsign-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: obligationsign.com
  spf: true
hosts:
- cert_expires: Dec 21 02:53:52 2026 GMT
  host: obligationsign.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Obligationsign Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for obligationsign-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: obligationsign-com
provider_slug: obligationsign-com
slug: obligationsign-com-domain-security
source_filename: obligationsign-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: obligationsign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 02:53:52 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: obligationsign.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/obligationsign-com/security/obligationsign-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Governance
- Security
- Infrastructure
---
