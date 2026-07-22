---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: peoplise.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: logo.com.tr
  spf: true
hosts:
- cert_expires: Oct 16 16:18:02 2026 GMT
  host: peoplise.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 14:04:43 2026 GMT
  host: www.logo.com.tr
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peoplise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peoplise, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Peoplise
provider_slug: peoplise
slug: peoplise-domain-security
source_filename: peoplise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: peoplise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 16:18:02 2026 GMT\n  hsts: false\n- host: www.logo.com.tr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 14:04:43 2026 GMT\n  hsts: false\ndomains:\n- domain: peoplise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: logo.com.tr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peoplise/refs/heads/main/security/peoplise-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Human Resources
- HR Tech
- Recruitment
- Hiring
- Talent Acquisition
- Video Interview
- Onboarding
- SaaS
- Turkey
---
