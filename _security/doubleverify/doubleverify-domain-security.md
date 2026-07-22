---
description: ''
domains:
- caa:
  - 0 issuewild "pki.apple.com"
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:sre@doubleverify.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: doubleverify.com
  spf: true
hosts:
- cert_expires: Sep  6 11:43:12 2026 GMT
  host: doubleverify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doubleverify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DoubleVerify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DoubleVerify
provider_slug: doubleverify
slug: doubleverify-domain-security
source_filename: doubleverify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doubleverify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 11:43:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: doubleverify.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.apple.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:sre@doubleverify.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doubleverify/refs/heads/main/security/doubleverify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ad Verification
- Ad Measurement
- Media Quality
- Brand Suitability
- Viewability
- Attention Measurement
- Invalid Traffic
- Fraud Detection
- Contextual Targeting
- Programmatic Advertising
- Connected TV
- Social Media Measurement
- Commerce Media
- Publisher Analytics
- MRC Accredited
- AdTech
---
