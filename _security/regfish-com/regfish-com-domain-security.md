---
api_specs:
- filename: regfish-com-openapi-generated.yml
  format: yaml
  label: regfish API
  slug: regfish-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regfish-com/openapi/_ae-authored/regfish-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: regfish.com
  spf: true
hosts:
- cert_expires: Feb 17 06:04:17 2027 GMT
  host: regfish.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: regfish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for regfish, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: regfish
provider_slug: regfish-com
slug: regfish-com-domain-security
source_filename: regfish-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: regfish.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 06:04:17 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: regfish.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/regfish-com/security/regfish-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Domains
- Email Hosting
- Web Hosting
- DNS
- API
- Managed WordPress
- Agency Plans
---
