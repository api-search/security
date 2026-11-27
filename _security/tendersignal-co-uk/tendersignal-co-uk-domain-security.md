---
api_specs:
- filename: tendersignal-co-uk-openapi-generated.yml
  format: yaml
  label: TenderSignal API
  slug: tendersignal-co-uk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tendersignal-co-uk/openapi/_ae-authored/tendersignal-co-uk-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tendersignal.co.uk
  spf: true
hosts:
- cert_expires: Jan  6 15:04:05 2027 GMT
  host: tendersignal.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TenderSignal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TenderSignal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TenderSignal
provider_slug: tendersignal-co-uk
slug: tendersignal-co-uk-domain-security
source_filename: tendersignal-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tendersignal.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 15:04:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tendersignal.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tendersignal-co-uk/security/tendersignal-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Procurement
- UK
- B2B
- SaaS
---
