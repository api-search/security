---
description: ''
domains:
- caa:
  - 0 iodef "mailto:sysadmin@guardsquare.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: guardsquare.com
  spf: true
hosts:
- cert_expires: Oct  3 06:56:31 2026 GMT
  host: www.guardsquare.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 13:15:25 2026 GMT
  host: platform.guardsquare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Guardsquare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GuardSquare, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GuardSquare
provider_slug: guardsquare
slug: guardsquare-domain-security
source_filename: guardsquare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.guardsquare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:56:31 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: platform.guardsquare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:15:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: guardsquare.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:sysadmin@guardsquare.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guardsquare/refs/heads/main/security/guardsquare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobile App Security
- Application Security
- Code Obfuscation
- Runtime Application Self-Protection
- Mobile Application Security Testing
- App Hardening
- App Attestation
- Threat Monitoring
---
