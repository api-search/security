---
api_specs:
- filename: namiq-io-lattice-api-openapi.yml
  format: yaml
  label: NamiQ Lattice API
  slug: namiq-io-lattice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namiq-io/openapi/namiq-io-lattice-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: namiq.io
  spf: true
hosts:
- cert_expires: Jan  6 01:24:06 2027 GMT
  host: namiq.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NamiQ Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NamiQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NamiQ
provider_slug: namiq-io
slug: namiq-io-domain-security
source_filename: namiq-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: namiq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 01:24:06 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: namiq.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/namiq-io/security/namiq-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- IT Services
- Security
- Automation
- Small Business
---
