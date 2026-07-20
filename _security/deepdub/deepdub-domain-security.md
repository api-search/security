---
api_specs:
- filename: deepdub-api-openapi-original.json
  format: json
  label: Deepdub Text-to-Speech API
  slug: deepdub-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepdub/refs/heads/main/openapi/deepdub-api-openapi-original.json
- filename: deepdub-managed-dub-openapi-original.json
  format: json
  label: Deepdub Managed Dubbing API
  slug: deepdub-managed-dubbing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepdub/refs/heads/main/openapi/deepdub-managed-dub-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: deepdub.ai
  spf: true
- caa:
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: deepdub.app
  spf: false
hosts:
- cert_expires: Sep 27 03:13:21 2026 GMT
  host: deepdub.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: restapi.deepdub.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: dubbing.deepdub.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deepdub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deepdub, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Deepdub
provider_slug: deepdub
slug: deepdub-domain-security
source_filename: deepdub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deepdub.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 03:13:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: restapi.deepdub.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\n- host: dubbing.deepdub.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: deepdub.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: deepdub.app\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepdub/refs/heads/main/security/deepdub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Voice
- Text to Speech
- Dubbing
- Localization
- Speech Synthesis
- Voice Cloning
- Media
- Artificial Intelligence
- Audio
---
