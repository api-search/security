---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: data.gov.in
  spf: true
hosts:
- cert_expires: Sep 17 11:16:50 2026 GMT
  host: data.gov.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government India Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, India, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Open Government, India
provider_slug: open-government-india
slug: open-government-india-domain-security
source_filename: open-government-india-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.gov.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 11:16:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: data.gov.in\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-india/refs/heads/main/security/open-government-india-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Public APIs
---
