---
api_specs:
- filename: cloudtalk-openapi.json
  format: json
  label: CloudTalk API
  slug: cloudtalk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cloudtalk.io
  spf: true
hosts:
- cert_expires: Sep 18 21:32:58 2026 GMT
  host: www.cloudtalk.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 21:32:58 2026 GMT
  host: my.cloudtalk.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudtalk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudTalk, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CloudTalk
provider_slug: cloudtalk
slug: cloudtalk-domain-security
source_filename: cloudtalk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudtalk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 21:32:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.cloudtalk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 21:32:58 2026 GMT\n  hsts: null\ndomains:\n- domain: cloudtalk.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/security/cloudtalk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Communications
- Voice
- VoIP
- Call Center
- Contact Center
- CCaaS
- Telephony
- SMS
- Conversation Intelligence
---
