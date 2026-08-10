---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: booknook.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: booknooklearning.com
  spf: true
hosts:
- cert_expires: Oct 14 06:08:31 2026 GMT
  host: www.booknook.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: marketing site
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: api.booknooklearning.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  response_headers:
    content-security-policy: present
    referrer-policy: no-referrer
    x-content-type-options: nosniff
    x-frame-options: SAMEORIGIN
  role: production API service
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: app.booknooklearning.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: student/tutor single-page application
  tls_version: TLSv1.3
- cert_expires: Oct 18 05:15:26 2026 GMT
  host: help.booknook.com
  hsts: false
  https: true
  role: customer help center
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Booknook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BookNook, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BookNook
provider_slug: booknook
slug: booknook-domain-security
source_filename: booknook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + discovered BookNook hosts\nhosts:\n- host: www.booknook.com\n  role: marketing site\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 06:08:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.booknooklearning.com\n  role: production API service\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n  hsts_include_subdomains: true\n  response_headers:\n    x-content-type-options: nosniff\n    x-frame-options: SAMEORIGIN\n    referrer-policy: no-referrer\n    content-security-policy: present\n- host: app.booknooklearning.com\n  role: student/tutor single-page application\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.booknook.com\n  role: customer help center\n  https: true\n  tls_version:\
  \ TLSv1.3\n  cert_expires: Oct 18 05:15:26 2026 GMT\n  hsts: false\ndomains:\n- domain: booknook.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: booknooklearning.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nnotes:\n- booknooklearning.com apex fails to serve (525 SSL handshake failure at the edge); www.booknooklearning.com redirects to www.booknook.com.\n- No CAA record on either registrable domain, and DNSSEC is not signed on either.\n- DMARC is published at p=quarantine on both domains, not p=reject.\n- help.booknook.com serves no HSTS header.\n- The production API service sets a complete security-header set (CSP, nosniff, SAMEORIGIN, no-referrer) and HSTS with preload.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/booknook/refs/heads/main/security/booknook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- EdTech
- Tutoring
- K-12
- Learning Platform
- Reading
- Mathematics
- Student Data
- Rostering
---
