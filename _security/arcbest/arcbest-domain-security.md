---
api_specs:
- filename: arcbest-api.yaml
  format: yaml
  label: ArcBest API
  slug: arcbest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/openapi/arcbest-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arcbest.com
  spf: true
hosts:
- cert_expires: Aug 22 09:35:04 2026 GMT
  host: www.arcbest.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.arcbest.com
  https: false
kind: domain-security
layout: security
method: probed
name: Arcbest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ArcBest, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ArcBest
provider_slug: arcbest
slug: arcbest-domain-security
source_filename: arcbest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arcbest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 09:35:04 2026 GMT\n  hsts: false\n- host: api.arcbest.com\n  https: false\ndomains:\n- domain: arcbest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcbest/refs/heads/main/security/arcbest-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Logistics
- Freight
- LTL
- Supply Chain
- Shipping
- Transportation
---
