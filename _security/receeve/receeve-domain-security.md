---
api_specs:
- filename: receeve-openapi-original.yml
  format: yaml
  label: Receive Client API
  slug: receive-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/openapi/receeve-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: receeve.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: receive-demo.com
  spf: false
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: api.receeve.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.receive-demo.com
  https: false
kind: domain-security
layout: security
method: probed
name: Receeve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Receeve, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Receeve
provider_slug: receeve
slug: receeve-domain-security
source_filename: receeve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.receeve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: false\n- host: api.receive-demo.com\n  https: false\ndomains:\n- domain: receeve.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: receive-demo.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/receeve/refs/heads/main/security/receeve-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Debt Collection
- Receivables Management
- Debt Servicing
- Collections
- Fintech
- Payments
- Webhooks
- Financial Services
- Dunning
---
