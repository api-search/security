---
description: ''
domains:
- caa:
  - 0 issuewild "rapidssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cloudbees.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: launchableinc.com
  spf: true
hosts:
- cert_expires: Sep 22 03:44:47 2026 GMT
  host: www.cloudbees.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 19:17:00 2026 GMT
  host: help.launchableinc.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.mercury.launchableinc.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Launchable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Launchable, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Launchable
provider_slug: launchable
slug: launchable-domain-security
source_filename: launchable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudbees.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:44:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.launchableinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 19:17:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mercury.launchableinc.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cloudbees.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"rapidssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: launchableinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/launchable/refs/heads/main/security/launchable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Continuous Integration
- Testing
- Test Automation
- Developer Tools
- DevOps
- Machine Learning
- Software Delivery
- Predictive Test Selection
- CI/CD
---
