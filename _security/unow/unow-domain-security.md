---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: unow.com
  mx:
  - smtp.google.com
  nameservers:
  - dns101.register.com
  - dns102.register.com
  spf: false
hosts:
- cert_expired: true
  cert_issuer: Sectigo RSA Domain Validation Secure Server CA
  cert_not_after: '2022-09-12'
  cert_subject_cn: '*.hostingplatform.com'
  cert_valid: false
  host: unow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  redirect_status: 301
  redirect_target_status: 404
  redirects_to: http://www.newuni.com/
- cert_subject_cn: '*.hostingplatform.com'
  cert_valid: false
  host: www.unow.com
  https: true
  redirects_to: http://www.newuni.com/
kind: domain-security
layout: security
method: probed
name: Unow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for uNow (UniversityNow), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS; 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: uNow (UniversityNow)
provider_slug: unow
slug: unow-domain-security
source_filename: unow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live probe of unow.com (dig + openssl s_client + curl)\nnote: >-\n  Company website is defunct. unow.com resolves and answers HTTPS but serves an\n  invalid, expired certificate (CN=*.hostingplatform.com, Sectigo, expired\n  2022-09-12) and 301-redirects everything to http://www.newuni.com/, which is a\n  Wix \"ConnectYourDomain Error\" 404 page. Google Workspace MX records remain\n  active on the domain.\nhosts:\n  - host: unow.com\n    https: true\n    cert_valid: false\n    cert_subject_cn: '*.hostingplatform.com'\n    cert_issuer: Sectigo RSA Domain Validation Secure Server CA\n    cert_expired: true\n    cert_not_after: '2022-09-12'\n    hsts: true\n    hsts_max_age: 31536000\n    redirects_to: http://www.newuni.com/\n    redirect_status: 301\n    redirect_target_status: 404\n  - host: www.unow.com\n    https: true\n    cert_valid: false\n    cert_subject_cn: '*.hostingplatform.com'\n    redirects_to: http://www.newuni.com/\n\
  domains:\n  - domain: unow.com\n    dnssec: false\n    caa: []\n    spf: false\n    dmarc: false\n    dmarc_policy: null\n    mx: [smtp.google.com]\n    nameservers: [dns101.register.com, dns102.register.com]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unow/refs/heads/main/security/unow-domain-security.yml
summary_line: HSTS
tags:
- Company
- Education
- Higher Education
- EdTech
- Online Learning
- Competency-Based Education
- Defunct
---
