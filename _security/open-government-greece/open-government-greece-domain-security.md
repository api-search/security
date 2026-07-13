---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: data.gov.gr
  spf: false
hosts:
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: data.gov.gr
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Open Government Greece Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Greece, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Open Government, Greece
provider_slug: open-government-greece
slug: open-government-greece-domain-security
source_filename: open-government-greece-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.gov.gr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: data.gov.gr\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-greece/refs/heads/main/security/open-government-greece-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Government
- Public APIs
---
