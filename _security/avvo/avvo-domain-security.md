---
api_specs:
- filename: avvo-openapi-generated.yml
  format: yaml
  label: Avvo API
  slug: avvo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avvo/openapi/_ae-authored/avvo-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: avvo.com
  spf: true
hosts:
- cert_expires: Dec 10 03:45:42 2026 GMT
  host: www.avvo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avvo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avvo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Avvo
provider_slug: avvo
slug: avvo-domain-security
source_filename: avvo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avvo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 03:45:42 2026 GMT\n  hsts: false\ndomains:\n- domain: avvo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/avvo/security/avvo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- LegalTech
- Marketplace
- Directory
- Reviews
- ConsumerServices
---
