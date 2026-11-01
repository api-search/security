---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:itsupport@anywhere.co"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: answerconnect.com
  spf: true
hosts:
- cert_expires: Dec 17 12:14:28 2026 GMT
  host: answerconnect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Answerconnect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AnswerConnect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AnswerConnect
provider_slug: answerconnect
slug: answerconnect-domain-security
source_filename: answerconnect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: answerconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 12:14:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: answerconnect.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:itsupport@anywhere.co\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/answerconnect/security/answerconnect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Call Answering
- Live Chat
- Appointment Scheduling
- Virtual Receptionist
- Integration
---
