---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spirashealth.com
  spf: true
hosts:
- cert_expires: Dec 29 11:25:51 2026 GMT
  host: spirashealth.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Spiras Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spiras Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Spiras Health
provider_slug: spiras-health
slug: spiras-health-domain-security
source_filename: spiras-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spirashealth.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 29 11:25:51 2026 GMT\n  hsts: false\ndomains:\n- domain: spirashealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/spiras-health/security/spiras-health-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Home-based care
- Nurse practitioner services
- Health plans
- Patient services
---
