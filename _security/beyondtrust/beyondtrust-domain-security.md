---
api_specs:
- filename: beyondtrust-password-safe-api.yaml
  format: yaml
  label: BeyondTrust Password Safe API
  slug: beyondtrust-password-safe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/openapi/beyondtrust-password-safe-api.yaml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:bt-administrator@beyondtrust.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: beyondtrust.com
  spf: true
hosts:
- cert_expires: Sep  5 14:50:06 2026 GMT
  host: docs.beyondtrust.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beyondtrust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BeyondTrust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BeyondTrust
provider_slug: beyondtrust
slug: beyondtrust-domain-security
source_filename: beyondtrust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.beyondtrust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 14:50:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: beyondtrust.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:bt-administrator@beyondtrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/security/beyondtrust-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
---
