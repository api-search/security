---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: revenue.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ringdna.com
  spf: true
hosts:
- cert_expires: Aug 26 07:54:15 2026 GMT
  host: www.revenue.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: support.revenue.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.ringdna.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ringdna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RingDNA, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: RingDNA
provider_slug: ringdna
slug: ringdna-domain-security
source_filename: ringdna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.revenue.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 07:54:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.revenue.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ringdna.com\n  https: false\ndomains:\n- domain: revenue.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ringdna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ringdna/refs/heads/main/security/ringdna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Sales Engagement
- Conversation Intelligence
- Sales Dialing
- Call Recording
- Revenue Orchestration
- CRM Integration
- Salesforce
- AI Coaching
- Sales Automation
---
