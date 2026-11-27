---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moneychoice.us
  spf: true
hosts:
- cert_expires: Jan 24 01:26:10 2027 GMT
  host: moneychoice.us
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MoneyChoice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MoneyChoice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MoneyChoice
provider_slug: moneychoice-us
slug: moneychoice-us-domain-security
source_filename: moneychoice-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moneychoice.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 01:26:10 2027 GMT\n  hsts: false\ndomains:\n- domain: moneychoice.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/moneychoice-us/security/moneychoice-us-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Software-as-a-Service
- Small Business
- Financial Management
- Automation
---
