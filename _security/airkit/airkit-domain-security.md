---
description: ''
domains:
- caa:
  - 0 iodef "mailto:caa-violations@salesforce.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: airkit.com
  spf: true
hosts:
- cert_expires: Oct 13 15:44:34 2026 GMT
  host: www.airkit.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airkit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AirKit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: AirKit
provider_slug: airkit
slug: airkit-domain-security
source_filename: airkit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airkit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 15:44:34 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: airkit.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:caa-violations@salesforce.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airkit/refs/heads/main/security/airkit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Automation
- Low-Code
- Customer Experience
- Conversational AI
- Acquired
- Salesforce
---
