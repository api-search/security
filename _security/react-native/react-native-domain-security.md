---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: reactnative.dev
  spf: true
hosts:
- cert_expires: Sep  5 05:53:52 2026 GMT
  host: reactnative.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: React Native Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for React Native, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: React Native
provider_slug: react-native
slug: react-native-domain-security
source_filename: react-native-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reactnative.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:53:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reactnative.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/react-native/refs/heads/main/security/react-native-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Android
- Cross-Platform
- iOS
- JavaScript
- Mobile Development
- Native Apps
- React
---
