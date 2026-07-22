---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 iodef "mailto:domains@featurespace.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: featurespace.com
  spf: true
hosts:
- cert_expires: Sep  7 14:27:14 2026 GMT
  host: www.featurespace.com
  hsts: true
  hsts_max_age: 264310
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Featurespace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Featurespace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Featurespace
provider_slug: featurespace
slug: featurespace-domain-security
source_filename: featurespace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.featurespace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 14:27:14 2026 GMT\n  hsts: true\n  hsts_max_age: 264310\ndomains:\n- domain: featurespace.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 iodef \"mailto:domains@featurespace.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/featurespace/refs/heads/main/security/featurespace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Prevention
- Fraud Detection
- Financial Crime
- Anti-Money Laundering
- Behavioral Analytics
- Risk Scoring
- Machine Learning
- Payments
- Company
---
