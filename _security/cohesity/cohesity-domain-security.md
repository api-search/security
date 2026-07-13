---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazontrust.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cohesity.com
  spf: true
hosts:
- cert_expires: Aug 20 09:38:01 2026 GMT
  host: www.cohesity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 18:23:48 2026 GMT
  host: developer.cohesity.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: helios.cohesity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cohesity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cohesity, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cohesity
provider_slug: cohesity
slug: cohesity-domain-security
source_filename: cohesity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cohesity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 09:38:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.cohesity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 18:23:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: helios.cohesity.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cohesity.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cohesity/refs/heads/main/security/cohesity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Backup
- Cyber Resilience
- Data Management
- Data Protection
- Data Security
- DataProtect
- Disaster Recovery
- Helios
- Orchestration
---
