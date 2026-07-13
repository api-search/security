---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "www.digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: forsta.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: focusvision.com
  spf: true
hosts:
- cert_expires: Sep 10 13:23:48 2026 GMT
  host: www.forsta.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: docs.developer.focusvision.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forsta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forsta, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Forsta
provider_slug: forsta
slug: forsta-domain-security
source_filename: forsta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.forsta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 13:23:48 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: docs.developer.focusvision.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: forsta.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"www.digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: focusvision.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forsta/refs/heads/main/security/forsta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Insights
- Feedback
- Market Research
---
