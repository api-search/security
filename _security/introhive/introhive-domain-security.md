---
description: ''
domains:
- caa:
  - 0 iodef "mailto:webmaster@introhive.com"
  - 0 issue "amazon.com"
  - 0 issue "comodo.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: introhive.com
  spf: true
hosts:
- cert_expires: Sep 27 06:23:28 2026 GMT
  host: www.introhive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: app.introhive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Introhive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Introhive, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Introhive
provider_slug: introhive
slug: introhive-domain-security
source_filename: introhive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.introhive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 06:23:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.introhive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: introhive.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:webmaster@introhive.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodo.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/introhive/refs/heads/main/security/introhive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Relationship Intelligence
- CRM
- Data Automation
- Contact Management
- Data Quality
- Professional Services
- Sales
- Enrichment
---
