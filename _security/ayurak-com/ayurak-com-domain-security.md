---
api_specs:
- filename: ayurak-com-openapi-generated.yml
  format: yaml
  label: ayurak-com API
  slug: ayurak-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayurak-com/openapi/_ae-authored/ayurak-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ayurak.com
  spf: true
hosts:
- cert_expires: Dec 19 03:35:56 2026 GMT
  host: ayurak.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ayurak Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ayurak-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ayurak-com
provider_slug: ayurak-com
slug: ayurak-com-domain-security
source_filename: ayurak-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ayurak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 03:35:56 2026 GMT\n  hsts: false\ndomains:\n- domain: ayurak.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ayurak-com/security/ayurak-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- AI
- Security
- Healthcare
- EmergencyResponse
- Technology
---
