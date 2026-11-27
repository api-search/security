---
api_specs:
- filename: jsmon-sh-openapi-generated.yml
  format: yaml
  label: Jsmon API
  slug: jsmon-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jsmon-sh/openapi/_ae-authored/jsmon-sh-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jsmon.sh
  spf: true
hosts:
- cert_expires: Jan 10 14:39:53 2027 GMT
  host: jsmon.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jsmon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jsmon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jsmon
provider_slug: jsmon-sh
slug: jsmon-sh-domain-security
source_filename: jsmon-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jsmon.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 14:39:53 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jsmon.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/jsmon-sh/security/jsmon-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Attack Surface
- Artificial Intelligence
- Monitoring
- Platform
---
