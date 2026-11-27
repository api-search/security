---
api_specs:
- filename: fixture-email-openapi-generated.yml
  format: yaml
  label: Fixture Email API
  slug: fixture-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixture-email/openapi/_ae-authored/fixture-email-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fixture.email
  spf: true
hosts:
- cert_expires: Jan 15 22:05:43 2027 GMT
  host: fixture.email
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fixture Email Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fixture Email, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fixture Email
provider_slug: fixture-email
slug: fixture-email-domain-security
source_filename: fixture-email-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fixture.email\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 22:05:43 2027 GMT\n  hsts: false\ndomains:\n- domain: fixture.email\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fixture-email/security/fixture-email-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Email
- Testing
- Artificial Intelligence
---
