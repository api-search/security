---
api_specs:
- filename: api.domestika.org
  format: yaml
  label: Domestika API
  slug: domestika-api
  spec_type: OpenAPI
  url: https://api.domestika.org
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: domestika.org
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: www.domestika.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.domestika.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Domestika Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Domestika, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Domestika
provider_slug: domestika
slug: domestika-domain-security
source_filename: domestika-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.domestika.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\n- host: api.domestika.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: domestika.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domestika/refs/heads/main/security/domestika-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Creative Education
- Online Learning
- Courses
- Design
- Photography
- Illustration
- Enterprise Learning
- REST API
---
