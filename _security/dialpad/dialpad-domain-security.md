---
api_specs:
- filename: dialpad-asyncapi.yml
  format: yaml
  label: Dialpad Webhooks API
  slug: dialpad-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/dialpad/refs/heads/main/openapi/dialpad-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:dns-admin@dialpad.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dialpad.com
  spf: true
hosts:
- cert_expires: Sep 26 18:47:20 2026 GMT
  host: www.dialpad.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 15:01:06 2026 GMT
  host: developers.dialpad.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: dialpad.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dialpad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dialpad, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dialpad
provider_slug: dialpad
slug: dialpad-domain-security
source_filename: dialpad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dialpad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 18:47:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.dialpad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:01:06 2026 GMT\n  hsts: null\n- host: dialpad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dialpad.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:dns-admin@dialpad.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dialpad/refs/heads/main/security/dialpad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communications
- Voice
- AI
- Contact Center
- UCaaS
---
