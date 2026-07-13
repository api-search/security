---
api_specs:
- filename: coralogix-asyncapi.yml
  format: yaml
  label: Coralogix
  slug: coralogix
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/coralogix/refs/heads/main/asyncapi/coralogix-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coralogix.com
  spf: true
hosts:
- cert_expires: Sep  8 21:11:27 2026 GMT
  host: coralogix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coralogix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coralogix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coralogix
provider_slug: coralogix
slug: coralogix-domain-security
source_filename: coralogix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coralogix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 21:11:27 2026 GMT\n  hsts: false\ndomains:\n- domain: coralogix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coralogix/refs/heads/main/security/coralogix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AIOps
- Observability
---
