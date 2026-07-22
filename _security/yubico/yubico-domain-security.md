---
api_specs:
- filename: yubico-yubicloud-openapi.yml
  format: yaml
  label: Yubico YubiCloud OTP Validation API
  slug: yubico-yubicloud-otp-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yubico/refs/heads/main/openapi/yubico-yubicloud-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 iodef "mailto:tlsadmin@yubico.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: yubico.com
  spf: true
hosts:
- cert_expires: Jan  8 18:52:06 2027 GMT
  host: yubico.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yubico Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yubico, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Yubico
provider_slug: yubico
slug: yubico-domain-security
source_filename: yubico-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yubico.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 18:52:06 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yubico.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:tlsadmin@yubico.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yubico/refs/heads/main/security/yubico-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Authentication
- Security
- Identity
- Hardware Security
- FIDO2
- WebAuthn
- One-Time Password
---
