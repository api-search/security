---
api_specs:
- filename: openphone-openapi-original.json
  format: json
  label: Quo Public API (OpenPhone)
  slug: quo-public-api-openphone
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openphone/refs/heads/main/openapi/openphone-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quo.com
  spf: true
hosts:
- cert_expires: Sep 23 05:54:28 2026 GMT
  host: www.quo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 05:54:28 2026 GMT
  host: api.quo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openphone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenPhone, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OpenPhone
provider_slug: openphone
slug: openphone-domain-security
source_filename: openphone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 05:54:28 2026 GMT\n  hsts: false\n- host: api.quo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 05:54:28 2026 GMT\n  hsts: null\ndomains:\n- domain: quo.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openphone/refs/heads/main/security/openphone-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Communications
- Voice
- SMS
- Messaging
- Telephony
- Business Phone
- CPaaS
- Contact Center
- Webhooks
---
