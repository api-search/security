---
api_specs:
- filename: entri-openapi-generated.yml
  format: yaml
  label: Entri API
  slug: entri-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entri/openapi/_ae-authored/entri-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: entri.com
  spf: true
hosts:
- cert_expires: Dec 17 10:11:18 2026 GMT
  host: entri.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Entri Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Entri, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Entri
provider_slug: entri
slug: entri-domain-security
source_filename: entri-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: entri.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 10:11:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: entri.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/entri/security/entri-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Domain
- Integration
- Software-as-a-Service
---
