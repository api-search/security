---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: medicalaialliance.org
  spf: true
hosts:
- cert_expires: Dec 23 06:27:12 2026 GMT
  host: medicalaialliance.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Medical AI Alliance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medical AI Alliance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Medical AI Alliance
provider_slug: medicalaialliance-org
slug: medicalaialliance-org-domain-security
source_filename: medicalaialliance-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medicalaialliance.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 06:27:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: medicalaialliance.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/medicalaialliance-org/security/medicalaialliance-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical AI
- Biotechnology
- Healthcare
- Consortium
---
