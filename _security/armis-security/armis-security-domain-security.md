---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: armis.com
  spf: true
hosts:
- cert_expires: Sep  5 19:01:23 2026 GMT
  host: www.armis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Armis Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Armis Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Armis Security
provider_slug: armis-security
slug: armis-security-domain-security
source_filename: armis-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.armis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 19:01:23 2026 GMT\n  hsts: null\ndomains:\n- domain: armis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armis-security/refs/heads/main/security/armis-security-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Cybersecurity
- Asset Intelligence
- Cyber Exposure Management
- IoT Security
- OT Security
- Application Security
---
