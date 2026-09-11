---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: justice.gov
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: www.justice.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Foreign Claims Settlement Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foreign Claims Settlement Commission, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Foreign Claims Settlement Commission
provider_slug: foreign-claims-settlement-commission
slug: foreign-claims-settlement-commission-domain-security
source_filename: foreign-claims-settlement-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  spf was re-verified by hand on 2026-09-10 after the probe's local resolver returned an empty TXT\n  set; justice.gov publishes \"v=spf1 -all\" (confirmed against 8.8.8.8, 1.1.1.1 and 9.9.9.9), so the\n  probe's spf:false was a resolver artifact and has been corrected. No CAA record is published.\nhosts:\n- host: www.justice.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: justice.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foreign-claims-settlement-commission/refs/heads/main/security/foreign-claims-settlement-commission-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Adjudication
- Claims
- Federal-Government
- International Claims
- Justice
- Legal
---
