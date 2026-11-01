---
api_specs:
- filename: uae-pass-openapi-generated.yml
  format: yaml
  label: UAE PASS API
  slug: uae-pass-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uae-pass/openapi/_ae-authored/uae-pass-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uaepass.ae
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: uaepass.ae
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Uae Pass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UAE PASS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UAE PASS
provider_slug: uae-pass
slug: uae-pass-domain-security
source_filename: uae-pass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uaepass.ae\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: uaepass.ae\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/uae-pass/security/uae-pass-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Identity
- Authentication
- UAE
- Digital
---
