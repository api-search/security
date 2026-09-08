---
description: ''
domains:
- caa:
  - 0 issuewild "pki.apple.com"
  - 0 iodef "mailto:contact_pki@apple.com"
  - 0 issue "pki.apple.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apple.com
  spf: true
hosts:
- cert_expires: Dec 16 18:31:25 2026 GMT
  host: www.apple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 19:03:17 2026 GMT
  host: developer.apple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Apple Safari Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apple Safari, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apple Safari
provider_slug: apple-safari
slug: apple-safari-domain-security
source_filename: apple-safari-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 18:31:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 19:03:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apple.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.apple.com\"\n  - 0 iodef \"mailto:contact_pki@apple.com\"\n  - 0 issue \"pki.apple.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apple-safari/refs/heads/main/security/apple-safari-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apple
- Browser
- Privacy
- Web Browser
- Webkit
---
