---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inferahealth.com
  spf: true
hosts:
- cert_expires: Dec 26 01:05:30 2026 GMT
  host: inferahealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Infera Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infera Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Infera Health
provider_slug: infera-health
slug: infera-health-domain-security
source_filename: infera-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inferahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 01:05:30 2026 GMT\n  hsts: false\ndomains:\n- domain: inferahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/infera-health/security/infera-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Compliance
- Medical Devices
- AI
- Software
- Risk Management
- Verification
- Release Management
- Document Control
---
