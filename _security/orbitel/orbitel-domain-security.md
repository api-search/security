---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: orbitel.in
  spf: true
hosts:
- cert_expires: Dec 30 08:22:05 2026 GMT
  host: orbitel.in
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Orbitel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orbitel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Orbitel
provider_slug: orbitel
slug: orbitel-domain-security
source_filename: orbitel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orbitel.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 08:22:05 2026 GMT\n  hsts: false\ndomains:\n- domain: orbitel.in\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbitel/refs/heads/main/security/orbitel-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- CPaaS
- Messaging
- SMS
- WhatsApp
- Voice
- Email
- RCS
---
