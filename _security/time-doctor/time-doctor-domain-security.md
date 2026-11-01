---
api_specs:
- filename: time-doctor-openapi-generated.yml
  format: yaml
  label: Time Doctor API
  slug: time-doctor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/time-doctor/openapi/_ae-authored/time-doctor-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:postmaster@timedoctordev.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: timedoctor.com
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: www.timedoctor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Time Doctor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Time Doctor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Time Doctor
provider_slug: time-doctor
slug: time-doctor-domain-security
source_filename: time-doctor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.timedoctor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: timedoctor.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:postmaster@timedoctordev.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/time-doctor/security/time-doctor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- TimeTracking
- WorkforceManagement
- Productivity
- AI
---
