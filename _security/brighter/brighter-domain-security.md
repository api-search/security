---
description: ''
domains:
- caa:
  - 0 issue "entrust.net"
  - 0 issue "godaddy.com"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:hostmaster@brighter.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brighter.com
  spf: true
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: brighter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brighter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brighter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brighter
provider_slug: brighter
slug: brighter-domain-security
source_filename: brighter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brighter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brighter.com\n  dnssec: false\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:hostmaster@brighter.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brighter/refs/heads/main/security/brighter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Dental
- Health Insurance
- Digital Health
- Benefits
- Appointment Scheduling
- Provider Directory
---
