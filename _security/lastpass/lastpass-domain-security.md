---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 iodef "mailto:domain@lastpass.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lastpass.com
  spf: true
hosts:
- cert_expires: Oct 24 12:51:12 2026 GMT
  host: www.lastpass.com
  hsts: true
  hsts_max_age: 86400000
  https: true
  tls_version: TLSv1.3
- host: support.lastpass.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- cert_expires: Oct 24 12:51:12 2026 GMT
  host: lastpass.com
  hsts: true
  hsts_max_age: 86400000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lastpass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LastPass, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LastPass
provider_slug: lastpass
slug: lastpass-domain-security
source_filename: lastpass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lastpass.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 12:51:12 2026 GMT\n  hsts: true\n  hsts_max_age: 86400000\n- host: support.lastpass.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: lastpass.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 12:51:12 2026 GMT\n  hsts: true\n  hsts_max_age: 86400000\ndomains:\n- domain: lastpass.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:domain@lastpass.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lastpass/refs/heads/main/security/lastpass-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Password Manager
- Vault
- Identity
- Enterprise
- SSO
- MFA
---
