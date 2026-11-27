---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cookie-script.com
  spf: true
hosts:
- cert_expires: Mar 21 23:59:59 2027 GMT
  host: cookie-script.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CookieScript Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CookieScript, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CookieScript
provider_slug: cookie-script
slug: cookie-script-domain-security
source_filename: cookie-script-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cookie-script.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cookie-script.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cookie-script/security/cookie-script-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cookie Consent
- GDPR Compliance
- Privacy Management
- Consent Management Platform
- Website Compliance
- Data Protection
---
