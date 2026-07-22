---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: evenuplaw.com
  spf: true
hosts:
- cert_expires: Sep 10 12:39:37 2026 GMT
  host: www.evenuplaw.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evenup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EvenUp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: EvenUp
provider_slug: evenup
slug: evenup-domain-security
source_filename: evenup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evenuplaw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 12:39:37 2026 GMT\n  hsts: false\ndomains:\n- domain: evenuplaw.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evenup/refs/heads/main/security/evenup-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Legal
- Legal Tech
- Personal Injury
- Plaintiff Law
- Case Management
- Demand Letters
- Medical Records
- AI Drafting
- Workflow Automation
- Settlement
- Litigation
- SaaS
---
