---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uscirf.gov
  spf: true
hosts:
- cert_expires: Oct  3 04:24:40 2026 GMT
  host: www.uscirf.gov
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Commission On International Religious Freedom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Commission on International Religious Freedom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: US Commission on International Religious Freedom
provider_slug: us-commission-on-international-religious-freedom
slug: us-commission-on-international-religious-freedom-domain-security
source_filename: us-commission-on-international-religious-freedom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uscirf.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 04:24:40 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\ndomains:\n- domain: uscirf.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-commission-on-international-religious-freedom/refs/heads/main/security/us-commission-on-international-religious-freedom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Federal Government
- Religious Freedom
- International Human Rights
- Foreign Policy
---
