---
api_specs:
- filename: dropwizard-admin.json
  format: json
  label: Dropwizard
  slug: dropwizard
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dropwizard/refs/heads/main/openapi/dropwizard-admin.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dropwizard.io
  spf: false
hosts:
- cert_expires: Aug 21 22:32:34 2026 GMT
  host: www.dropwizard.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dropwizard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dropwizard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Dropwizard
provider_slug: dropwizard
slug: dropwizard-domain-security
source_filename: dropwizard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dropwizard.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 22:32:34 2026 GMT\n  hsts: false\ndomains:\n- domain: dropwizard.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dropwizard/refs/heads/main/security/dropwizard-domain-security.yml
summary_line: TLSv1.3
tags:
- API Development
- Frameworks
- Java
- Microservices
- REST
- Web Services
---
