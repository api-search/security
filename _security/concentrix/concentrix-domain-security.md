---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: concentrix.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ixhello.com
  spf: true
hosts:
- cert_expires: Nov 23 18:41:18 2026 GMT
  host: www.concentrix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 10:35:35 2026 GMT
  host: docs.ixhello.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: api.vnext.ixhello.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Concentrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Concentrix, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Concentrix
provider_slug: concentrix
slug: concentrix-domain-security
source_filename: concentrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.concentrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 18:41:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ixhello.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 10:35:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.vnext.ixhello.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: concentrix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ixhello.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/concentrix/refs/heads/main/security/concentrix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Business Process Outsourcing
- Consulting
- Conversational AI
- Customer Experience
- Digital Transformation
- Enterprise Services
- Contact Center
- Voice
- Webhooks
- Fortune 500
---
