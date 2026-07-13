---
api_specs:
- filename: talkdesk-webhooks-asyncapi.yml
  format: yaml
  label: Talkdesk Webhook Surface
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkdesk/refs/heads/main/asyncapi/talkdesk-webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 128 iodef "mailto:domain-names@talkdesk.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: talkdesk.com
  spf: true
hosts:
- cert_expires: Oct  5 08:02:35 2026 GMT
  host: www.talkdesk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 20:16:33 2026 GMT
  host: docs.talkdesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Talkdesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Talkdesk, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Talkdesk
provider_slug: talkdesk
slug: talkdesk-domain-security
source_filename: talkdesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.talkdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 08:02:35 2026 GMT\n  hsts: false\n- host: docs.talkdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:16:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: talkdesk.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 128 iodef \"mailto:domain-names@talkdesk.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talkdesk/refs/heads/main/security/talkdesk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Contact Center
- CCaaS
- Voice
- Webhooks
- Events
- Telephony
- Customer Experience
- Digital Connect
- AppConnect
---
