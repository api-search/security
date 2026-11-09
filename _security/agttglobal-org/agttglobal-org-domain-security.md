---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agttglobal.org
  spf: false
hosts:
- cert_expires: Dec 23 11:33:34 2026 GMT
  host: agttglobal.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agttglobal Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rose Bounty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Rose Bounty
provider_slug: agttglobal-org
slug: agttglobal-org-domain-security
source_filename: agttglobal-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agttglobal.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 11:33:34 2026 GMT\n  hsts: null\ndomains:\n- domain: agttglobal.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agttglobal-org/security/agttglobal-org-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Verification
- Autonomous
- Payments
- Platform
---
