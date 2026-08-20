---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: associatedbank.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: jackhenry.dev
  spf: false
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: www.associatedbank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 20:00:04 2026 GMT
  host: jackhenry.dev
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Associated Banc Corp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Associated Bank, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Associated Bank
provider_slug: associated-banc-corp
slug: associated-banc-corp-domain-security
source_filename: associated-banc-corp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.associatedbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: jackhenry.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 20:00:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: associatedbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: jackhenry.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/associated-banc-corp/refs/heads/main/security/associated-banc-corp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- United States
- Regional Bank
- Commercial Banking
- Data Aggregation
- Open Finance
---
