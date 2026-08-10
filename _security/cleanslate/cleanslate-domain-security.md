---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cleanslatecenters.com
  spf: true
hosts:
- cert_expires: Sep 24 21:58:25 2026 GMT
  host: www.cleanslatecenters.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cleanslate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CleanSlate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CleanSlate
provider_slug: cleanslate
slug: cleanslate-domain-security
source_filename: cleanslate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cleanslatecenters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:58:25 2026 GMT\n  hsts: false\ndomains:\n- domain: cleanslatecenters.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleanslate/refs/heads/main/security/cleanslate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Behavioral Health
- Addiction Treatment
- Opioid Use Disorder
- Medication-Assisted Treatment
- Outpatient Clinics
- United States
---
