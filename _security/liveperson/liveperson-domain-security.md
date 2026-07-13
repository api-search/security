---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: liveperson.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: liveperson.net
  spf: true
hosts:
- cert_expires: Aug 15 18:24:14 2026 GMT
  host: www.liveperson.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 14:21:44 2026 GMT
  host: developers.liveperson.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: api.liveperson.net
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Liveperson Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LivePerson, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LivePerson
provider_slug: liveperson
slug: liveperson-domain-security
source_filename: liveperson-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liveperson.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 18:24:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.liveperson.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:21:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.liveperson.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: liveperson.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: liveperson.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liveperson/refs/heads/main/security/liveperson-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Conversational AI
- Customer Engagement
- Messaging
- Contact Center
- Bots
- Chat
---
