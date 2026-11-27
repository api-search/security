---
api_specs:
- filename: gethostwatch-com-openapi-generated.yml
  format: yaml
  label: Hostwatch API
  slug: gethostwatch-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gethostwatch-com/openapi/_ae-authored/gethostwatch-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gethostwatch.com
  spf: false
hosts:
- cert_expires: Dec 10 14:51:18 2026 GMT
  host: gethostwatch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hostwatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hostwatch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Hostwatch
provider_slug: gethostwatch-com
slug: gethostwatch-com-domain-security
source_filename: gethostwatch-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gethostwatch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 14:51:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gethostwatch.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/gethostwatch-com/security/gethostwatch-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Infrastructure
- Monitoring
- Security
- Cloud
- PrivateEnterprise
---
