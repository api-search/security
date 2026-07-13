---
api_specs:
- filename: swagger.yaml
  format: yaml
  label: ClickSend REST API v3
  slug: rest-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ClickSend/clicksend-go/master/api/swagger.yaml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clicksend.com
  spf: true
hosts:
- cert_expires: Aug 24 20:43:31 2026 GMT
  host: www.clicksend.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: developers.clicksend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 03:28:03 2026 GMT
  host: rest.clicksend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clicksend Sms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClickSend SMS, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ClickSend SMS
provider_slug: clicksend-sms
slug: clicksend-sms-domain-security
source_filename: clicksend-sms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clicksend.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 24 20:43:31 2026 GMT\n  hsts: false\n- host: developers.clicksend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\n- host: rest.clicksend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 03:28:03 2026 GMT\n  hsts: false\ndomains:\n- domain: clicksend.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clicksend-sms/refs/heads/main/security/clicksend-sms-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- SMS
- MMS
- Messaging
- Voice
- Email
- Fax
- Direct Mail
- Communications
---
