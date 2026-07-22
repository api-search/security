---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:domain_name_admins+dns@vital.io"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vital.io
  spf: true
hosts:
- cert_expires: Sep 14 16:24:21 2026 GMT
  host: vital.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vitaler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Vital
provider_slug: vitaler
slug: vitaler-domain-security
source_filename: vitaler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vital.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 16:24:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vital.io\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:domain_name_admins+dns@vital.io\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vitaler/refs/heads/main/security/vitaler-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Patient Experience
- EHR
- FHIR
- HL7
- Hospital
- Digital Health
- HITRUST
- Care Coordination
---
