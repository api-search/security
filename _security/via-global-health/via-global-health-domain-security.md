---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: viaglobalhealth.com
  spf: true
hosts:
- cert_expires: Aug 26 06:12:56 2026 GMT
  host: viaglobalhealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Via Global Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Via Global Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Via Global Health
provider_slug: via-global-health
slug: via-global-health-domain-security
source_filename: via-global-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: viaglobalhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 06:12:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: viaglobalhealth.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/via-global-health/refs/heads/main/security/via-global-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Medical Devices
- Medical Equipment
- Healthcare
- Pharmaceuticals
- Supply Chain
- Global Health
- Africa
- E-Commerce
---
