---
api_specs:
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Voice API
  slug: telnyx-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Messaging API
  slug: telnyx-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Numbers API
  slug: telnyx-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Verify API
  slug: telnyx-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Fax API
  slug: telnyx-fax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Wireless API
  slug: telnyx-wireless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Networking API
  slug: telnyx-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx AI API
  slug: telnyx-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
- filename: telnyx-openapi.yml
  format: yaml
  label: Telnyx Billing & Reporting API
  slug: telnyx-billing-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/openapi/telnyx-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@telnyx.com"
  - 0 issue "alphassl.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: telnyx.com
  spf: true
hosts:
- cert_expires: Oct 31 13:43:45 2026 GMT
  host: telnyx.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 06:35:03 2026 GMT
  host: developers.telnyx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 10:27:40 2026 GMT
  host: api.telnyx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Telnyx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telnyx, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Telnyx
provider_slug: telnyx
slug: telnyx-domain-security
source_filename: telnyx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: telnyx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 13:43:45 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: developers.telnyx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:35:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.telnyx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 10:27:40 2026 GMT\n  hsts: null\ndomains:\n- domain: telnyx.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@telnyx.com\"\n  - 0 issue \"alphassl.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telnyx/refs/heads/main/security/telnyx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communications
- CPaaS
- Voice
- SMS
- IoT
---
