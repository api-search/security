---
api_specs:
- filename: google-patents-openapi-generated.yml
  format: yaml
  label: Google Patents API
  slug: google-patents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-patents/refs/heads/main/openapi/_ae-authored/google-patents-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Dec 11 20:00:10 2026 GMT
  host: patents.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Google Patents Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Patents, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Patents
provider_slug: google-patents
slug: google-patents-domain-security
source_filename: google-patents-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: patents.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 20:00:10 2026 GMT\n  hsts: false\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-patents/refs/heads/main/security/google-patents-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Patents
- Search
- Intellectual-Property
- Google
---
