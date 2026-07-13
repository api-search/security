---
api_specs:
- filename: friendly-captcha-openapi.yml
  format: yaml
  label: Friendly Captcha Siteverify API
  slug: siteverify
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/friendly-captcha/refs/heads/main/openapi/friendly-captcha-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: friendlycaptcha.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: frcapi.com
  spf: false
hosts:
- cert_expires: Sep 20 06:39:13 2026 GMT
  host: friendlycaptcha.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 04:47:07 2026 GMT
  host: developer.friendlycaptcha.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: global.frcapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Friendly Captcha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Friendly Captcha, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Friendly Captcha
provider_slug: friendly-captcha
slug: friendly-captcha-domain-security
source_filename: friendly-captcha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: friendlycaptcha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 06:39:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.friendlycaptcha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 04:47:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: global.frcapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: friendlycaptcha.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: frcapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/friendly-captcha/refs/heads/main/security/friendly-captcha-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CAPTCHA
- Bot Defense
- Privacy
- Proof of Work
- GDPR
- European Hosting
- Accessibility
---
