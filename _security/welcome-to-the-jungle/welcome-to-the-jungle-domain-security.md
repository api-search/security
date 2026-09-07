---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: welcometothejungle.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: welcomekit.co
  spf: true
hosts:
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: www.welcometothejungle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 15:46:54 2026 GMT
  host: developers.welcomekit.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: www.welcomekit.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Welcome To The Jungle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Welcome to the Jungle, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Welcome to the Jungle
provider_slug: welcome-to-the-jungle
slug: welcome-to-the-jungle-domain-security
source_filename: welcome-to-the-jungle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.welcometothejungle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: null\n- host: developers.welcomekit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 15:46:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.welcomekit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: welcometothejungle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: welcomekit.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/welcome-to-the-jungle/refs/heads/main/security/welcome-to-the-jungle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Human Resources
- Recruiting
- Applicant Tracking
- Jobs
- Employer Branding
- Talent Acquisition
- HR Tech
- France
---
