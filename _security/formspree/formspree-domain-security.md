---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: formspree.io
  spf: true
hosts:
- cert_expires: Sep 24 00:45:16 2026 GMT
  host: formspree.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 00:45:16 2026 GMT
  host: help.formspree.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Formspree Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Formspree, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Formspree
provider_slug: formspree
slug: formspree-domain-security
source_filename: formspree-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formspree.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 00:45:16 2026 GMT\n  hsts: false\n- host: help.formspree.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 00:45:16 2026 GMT\n  hsts: false\ndomains:\n- domain: formspree.io\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formspree/refs/heads/main/security/formspree-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Forms
- Backend
- Static Sites
- Email
- Webhooks
- JAMstack
- CLI
---
