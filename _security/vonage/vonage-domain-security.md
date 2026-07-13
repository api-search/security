---
api_specs:
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage SMS API
  slug: vonage-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage Voice API
  slug: vonage-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage Messages API
  slug: vonage-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage Verify API
  slug: vonage-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage Numbers API
  slug: vonage-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage Application API
  slug: vonage-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: vonage.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nexmo.com
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: developer.vonage.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 20:11:55 2026 GMT
  host: www.vonage.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: rest.nexmo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vonage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vonage, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Vonage
provider_slug: vonage
slug: vonage-domain-security
source_filename: vonage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.vonage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.vonage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:11:55 2026 GMT\n  hsts: null\n- host: rest.nexmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: vonage.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nexmo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/security/vonage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Communication
- Messaging
- Telecommunications
- Video Conferencing
- Voice
- SMS
- Verification
---
