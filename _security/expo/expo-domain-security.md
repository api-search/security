---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: expo.dev
  spf: true
hosts:
- cert_expires: Oct  5 17:36:46 2026 GMT
  host: expo.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 21:56:41 2026 GMT
  host: docs.expo.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 07:36:36 2026 GMT
  host: api.expo.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Expo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Expo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Expo
provider_slug: expo
slug: expo-domain-security
source_filename: expo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: expo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 17:36:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.expo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 21:56:41 2026 GMT\n  hsts: false\n- host: api.expo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 07:36:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: expo.dev\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expo/refs/heads/main/security/expo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- React Native
- Mobile Development
- Build Automation
- Over-the-Air Updates
- CI/CD
- App Store Submission
- Push Notifications
- Cloud Build
- Developer Tools
---
