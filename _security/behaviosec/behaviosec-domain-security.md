---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: false
  dnssec: true
  domain: behaviosec.com
  spf: true
hosts:
- cert_expires: Dec 25 16:41:22 2026 GMT
  host: www.behaviosec.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Behaviosec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BehavioSec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: BehavioSec
provider_slug: behaviosec
slug: behaviosec-domain-security
source_filename: behaviosec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.behaviosec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 16:41:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: behaviosec.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/behaviosec/refs/heads/main/security/behaviosec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Enterprise
- Behavioral Biometrics
- Fraud Detection
- Authentication
- Identity
- Security
- Risk
- Continuous Authentication
---
