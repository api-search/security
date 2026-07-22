---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getrhyme.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: priorauthnow.com
  spf: true
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: getrhyme.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 04:29:51 2026 GMT
  host: www.priorauthnow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rhyme Fka Priorauthnow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rhyme (fka PriorAuthNow), probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rhyme (fka PriorAuthNow)
provider_slug: rhyme-fka-priorauthnow
slug: rhyme-fka-priorauthnow-domain-security
source_filename: rhyme-fka-priorauthnow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getrhyme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: false\n- host: www.priorauthnow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 04:29:51 2026 GMT\n  hsts: false\ndomains:\n- domain: getrhyme.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: priorauthnow.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhyme-fka-priorauthnow/refs/heads/main/security/rhyme-fka-priorauthnow-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Prior Authorization
- Health IT
- Payers
- Providers
- Revenue Cycle
- Automation
---
