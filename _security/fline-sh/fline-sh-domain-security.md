---
api_specs:
- filename: fline-sh-openapi-generated.yml
  format: yaml
  label: fline API
  slug: fline-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fline-sh/openapi/_ae-authored/fline-sh-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fline.sh
  spf: true
hosts:
- cert_expires: Jan 15 07:24:15 2027 GMT
  host: fline.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: fline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fline, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: fline
provider_slug: fline-sh
slug: fline-sh-domain-security
source_filename: fline-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fline.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 07:24:15 2027 GMT\n  hsts: false\ndomains:\n- domain: fline.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fline-sh/security/fline-sh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Platform
- Deployment
- Artificial Intelligence
- Cloud
- PrivateBeta
---
