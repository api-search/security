---
api_specs:
- filename: globkurier-pl-openapi-generated.yml
  format: yaml
  label: GlobKurier API
  slug: globkurier-pl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globkurier-pl/openapi/_ae-authored/globkurier-pl-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: globkurier.pl
  spf: true
hosts:
- cert_expires: Apr 12 23:59:59 2027 GMT
  host: globkurier.pl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GlobKurier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GlobKurier, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GlobKurier
provider_slug: globkurier-pl
slug: globkurier-pl-domain-security
source_filename: globkurier-pl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: globkurier.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: globkurier.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/globkurier-pl/security/globkurier-pl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Couriers
- Poland
- Shipping
---
