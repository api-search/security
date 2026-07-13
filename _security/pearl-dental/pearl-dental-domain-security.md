---
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hellopearl.com
  spf: true
hosts:
- cert_expires: Sep 14 04:46:00 2026 GMT
  host: hellopearl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: management.hellopearl.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 06:03:02 2026 GMT
  host: www.hellopearl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pearl Dental Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pearl, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pearl
provider_slug: pearl-dental
slug: pearl-dental-domain-security
source_filename: pearl-dental-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hellopearl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:46:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: management.hellopearl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.hellopearl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 06:03:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hellopearl.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pearl-dental/refs/heads/main/security/pearl-dental-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Dental
- Computer Vision
- Radiology
- Medical Imaging
- Pathology Detection
- Healthcare
- Partner Gated
---
