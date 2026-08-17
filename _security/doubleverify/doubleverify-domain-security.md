---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "digicert.com"
  - 0 issuewild "amazon.com"
  - 0 issue "pki.goog"
  - 0 issuewild "pki.goog"
  - 0 issuewild "microsoft.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: doubleverify.com
  spf: true
hosts:
- cert_expires: Nov  4 11:11:05 2026 GMT
  host: doubleverify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 14:39:47 2026 GMT
  host: mcp.doubleverify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 13:10:47 2026 GMT
  host: developer.doubleverify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doubleverify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DoubleVerify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DoubleVerify
provider_slug: doubleverify
slug: doubleverify-domain-security
source_filename: doubleverify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doubleverify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 11:11:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.doubleverify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:39:47 2026 GMT\n  hsts: null\n- host: developer.doubleverify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 13:10:47 2026 GMT\n  hsts: false\ndomains:\n- domain: doubleverify.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
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
