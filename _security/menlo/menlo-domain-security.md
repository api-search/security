---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:seceng@menlosecurity.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: menlosecurity.com
  spf: true
hosts:
- cert_expires: Oct 14 05:47:21 2026 GMT
  host: www.menlosecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Menlo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Menlo Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Menlo Security
provider_slug: menlo
slug: menlo-domain-security
source_filename: menlo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.menlosecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 05:47:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: menlosecurity.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:seceng@menlosecurity.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/menlo/refs/heads/main/security/menlo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Cybersecurity
- Browser Security
- Enterprise Browser
- Browser Isolation
- Zero Trust
- Data Loss Prevention
- AI Agent Security
- Threat Prevention
---
