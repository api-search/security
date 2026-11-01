---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quincetx.com
  spf: true
hosts:
- cert_expires: Jan 10 11:20:39 2027 GMT
  host: quincetx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Quince Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quince Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Quince Therapeutics
provider_slug: quince-therapeutics
slug: quince-therapeutics-domain-security
source_filename: quince-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quincetx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 11:20:39 2027 GMT\n  hsts: false\ndomains:\n- domain: quincetx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/quince-therapeutics/security/quince-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Pulmonary Therapeutics
- mTOR
- Clinical Trials
---
