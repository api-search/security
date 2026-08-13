---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anonymco.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: anonymportal.com
  spf: true
  spf_record: v=spf1 include:_spf.firebasemail.com include:mailgun.org ~all
- caa: []
  dmarc: false
  dnssec: true
  domain: anonymapis.com
  spf: false
hosts:
- cert_expires: Oct 16 07:40:57 2026 GMT
  host: anonymco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 21:33:05 2026 GMT
  host: anonymportal.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  note: Customer Transparency Portal. Serves a strict Content-Security-Policy with frame-ancestors 'self', default-src 'self', object-src 'none', base-uri 'self', form-action 'self', plus X-Frame-Options DENY, X-Content-Type-Options nosniff, Referrer-Policy no-referrer and a Permissions-Policy restricting camera and microphone. Notably strong header posture.
  tls_version: TLSv1.3
- cert_expires: null
  host: anonymapis.com
  hsts: unknown
  https: unknown
  note: The gRPC API host declared in the portal's own environment config and CSP connect-src. Resolves to 52.230.151.22 (Microsoft Azure) but TCP 443 does not complete from the public internet, so no TLS or header posture can be measured. Firewalled, not absent.
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Anonymco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anonym, probed live across 3 host(s) and 3 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Anonym
provider_slug: anonymco
slug: anonymco-domain-security
source_filename: anonymco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the two API/portal hosts named in Anonym's own published portal configuration\nhosts:\n- host: anonymco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 07:40:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: anonymportal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 21:33:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n  note: >-\n    Customer Transparency Portal. Serves a strict Content-Security-Policy with frame-ancestors\n    'self', default-src 'self', object-src 'none', base-uri 'self', form-action 'self', plus\n    X-Frame-Options DENY, X-Content-Type-Options nosniff, Referrer-Policy no-referrer and a\n    Permissions-Policy restricting camera and microphone. Notably strong header posture.\n- host: anonymapis.com\n  https: unknown\n  tls_version: null\n  cert_expires: null\n  hsts: unknown\n  note: >-\n    The gRPC API\
  \ host declared in the portal's own environment config and CSP connect-src. Resolves\n    to 52.230.151.22 (Microsoft Azure) but TCP 443 does not complete from the public internet, so\n    no TLS or header posture can be measured. Firewalled, not absent.\ndomains:\n- domain: anonymco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: anonymportal.com\n  dnssec: true\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.firebasemail.com include:mailgun.org ~all\n  dmarc: false\n- domain: anonymapis.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\nfindings:\n- All three domains publish no CAA record, so no certificate authority is pinned.\n- anonymco.com has SPF and a quarantine DMARC policy but no DNSSEC.\n- anonymportal.com and anonymapis.com are DNSSEC-signed but anonymportal.com publishes no DMARC record.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anonymco/refs/heads/main/security/anonymco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Advertising
- Advertising Technology
- Privacy
- Ad Measurement
- Confidential Computing
- Mozilla
- Attribution
- Differential Privacy
- Trusted Execution Environment
- Marketing
---
