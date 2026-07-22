---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sni.cloudflaressl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: boundless.com
  spf: true
hosts:
- cert_expires: Sep 15 07:51:09 2026 GMT
  host: www.boundless.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boundless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boundless, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Boundless
provider_slug: boundless
slug: boundless-domain-security
source_filename: boundless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boundless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:51:09 2026 GMT\n  hsts: false\ndomains:\n- domain: boundless.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sni.cloudflaressl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boundless/refs/heads/main/security/boundless-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Immigration Tech
- Immigration
- Legal Tech
- Visas
- Green Cards
- Citizenship
- Global Mobility
- Case Management
---
