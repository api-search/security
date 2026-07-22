---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: speak.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: usespeak.com
  spf: true
hosts:
- cert_expires: Oct 17 07:24:01 2026 GMT
  host: www.speak.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 09:34:58 2026 GMT
  host: api.usespeak.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Speak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Speak, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Speak
provider_slug: speak
slug: speak-domain-security
source_filename: speak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.speak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 07:24:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.usespeak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 09:34:58 2026 GMT\n  hsts: false\ndomains:\n- domain: speak.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: usespeak.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speak/refs/heads/main/security/speak-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Language Learning
- Education
- EdTech
- Speech
- Conversational AI
- Mobile
---
