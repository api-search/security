---
api_specs:
- filename: signal-accounts-api-openapi.yml
  format: yaml
  label: Signal Accounts API
  slug: signal-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal/refs/heads/main/openapi/signal-accounts-api-openapi.yml
- filename: signal-attachments-api-openapi.yml
  format: yaml
  label: Signal Attachments API
  slug: signal-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal/refs/heads/main/openapi/signal-attachments-api-openapi.yml
- filename: signal-certificates-api-openapi.yml
  format: yaml
  label: Signal Certificates API
  slug: signal-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal/refs/heads/main/openapi/signal-certificates-api-openapi.yml
- filename: signal-devices-api-openapi.yml
  format: yaml
  label: Signal Devices API
  slug: signal-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal/refs/heads/main/openapi/signal-devices-api-openapi.yml
- filename: signal-keys-api-openapi.yml
  format: yaml
  label: Signal Keys API
  slug: signal-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal/refs/heads/main/openapi/signal-keys-api-openapi.yml
- filename: signal-messages-api-openapi.yml
  format: yaml
  label: Signal Messages API
  slug: signal-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal/refs/heads/main/openapi/signal-messages-api-openapi.yml
- filename: signal-profiles-api-openapi.yml
  format: yaml
  label: Signal Profiles API
  slug: signal-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal/refs/heads/main/openapi/signal-profiles-api-openapi.yml
- filename: signal-registration-api-openapi.yml
  format: yaml
  label: Signal Registration API
  slug: signal-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal/refs/heads/main/openapi/signal-registration-api-openapi.yml
- filename: signal-stickers-api-openapi.yml
  format: yaml
  label: Signal Stickers API
  slug: signal-stickers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signal/refs/heads/main/openapi/signal-stickers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: signal.org
  spf: true
hosts:
- cert_expires: Oct  5 17:16:42 2026 GMT
  host: signal.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: chat.signal.org
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Signal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Signal, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Signal
provider_slug: signal
slug: signal-domain-security
source_filename: signal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: signal.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 17:16:42 2026 GMT\n  hsts: false\n- host: chat.signal.org\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: signal.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signal/refs/heads/main/security/signal-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Encryption
- Messaging
- Security
- Cryptography
- Open-Source
- Privacy
---
