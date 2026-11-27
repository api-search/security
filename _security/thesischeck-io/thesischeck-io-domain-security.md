---
api_specs:
- filename: thesischeck-io-openapi-generated.yml
  format: yaml
  label: ThesisCheck API
  slug: thesischeck-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thesischeck-io/openapi/_ae-authored/thesischeck-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: true
  domain: thesischeck.io
  spf: true
hosts:
- cert_expires: Jan 27 19:59:00 2027 GMT
  host: thesischeck.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ThesisCheck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThesisCheck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ThesisCheck
provider_slug: thesischeck-io
slug: thesischeck-io-domain-security
source_filename: thesischeck-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thesischeck.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 19:59:00 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thesischeck.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/thesischeck-io/security/thesischeck-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Finance
- Investment
- Research
- Data
---
