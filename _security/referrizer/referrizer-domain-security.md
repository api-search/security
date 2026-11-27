---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: referrizer.com
  spf: true
hosts:
- cert_expires: Dec 25 17:05:39 2026 GMT
  host: referrizer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Referrizer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Referrizer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Referrizer
provider_slug: referrizer
slug: referrizer-domain-security
source_filename: referrizer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: referrizer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 17:05:39 2026 GMT\n  hsts: false\ndomains:\n- domain: referrizer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/referrizer/security/referrizer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Marketing Automation
- Referral Marketing
- Reputation Management
- Lead Management
- Loyalty Program
- Email Marketing
- SMS Marketing
- AI Assistant
---
