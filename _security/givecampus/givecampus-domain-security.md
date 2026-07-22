---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: givecampus.com
  spf: true
hosts:
- cert_expires: Oct 12 03:45:09 2026 GMT
  host: www.givecampus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Givecampus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Givecampus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Givecampus
provider_slug: givecampus
slug: givecampus-domain-security
source_filename: givecampus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.givecampus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:45:09 2026 GMT\n  hsts: null\ndomains:\n- domain: givecampus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/givecampus/refs/heads/main/security/givecampus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fundraising
- Nonprofit
- Education
- Advancement
- Alumni Engagement
- Donor Management
- Payments
- Giving
- CRM
---
