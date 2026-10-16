---
api_specs:
- filename: credorax-openapi-generated.yml
  format: yaml
  label: Credorax API
  slug: credorax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credorax/refs/heads/main/openapi/_ae-authored/credorax-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shift4.com
  spf: true
hosts:
- cert_expires: Nov 26 20:04:53 2026 GMT
  host: www.shift4.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Credorax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credorax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Credorax
provider_slug: credorax
slug: credorax-domain-security
source_filename: credorax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shift4.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 20:04:53 2026 GMT\n  hsts: null\ndomains:\n- domain: shift4.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credorax/refs/heads/main/security/credorax-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
