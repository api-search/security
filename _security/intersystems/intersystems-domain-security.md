---
api_specs:
- filename: intersystems-openapi-generated.yml
  format: yaml
  label: InterSystems API
  slug: intersystems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intersystems/refs/heads/main/openapi/_ae-authored/intersystems-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intersystems.com
  spf: true
hosts:
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: www.intersystems.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Intersystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InterSystems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: InterSystems
provider_slug: intersystems
slug: intersystems-domain-security
source_filename: intersystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.intersystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: intersystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intersystems/refs/heads/main/security/intersystems-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
