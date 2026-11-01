---
api_specs:
- filename: ayble-openapi-generated.yml
  format: yaml
  label: Ayble API
  slug: ayble-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayble/openapi/_ae-authored/ayble-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ayblehealth.com
  spf: true
hosts:
- cert_expires: Jan 27 09:52:25 2027 GMT
  host: www.ayblehealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ayble Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ayble, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ayble
provider_slug: ayble
slug: ayble-domain-security
source_filename: ayble-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ayblehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 09:52:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ayblehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ayble/security/ayble-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Telemedicine
- DigestiveHealth
- VirtualClinic
- EmployerBenefits
- Healthcare
---
