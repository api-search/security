---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: eucalyptus.health
  spf: true
hosts:
- cert_expires: Sep  9 23:26:11 2026 GMT
  host: www.eucalyptus.health
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eucalyptus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eucalyptus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Eucalyptus
provider_slug: eucalyptus
slug: eucalyptus-domain-security
source_filename: eucalyptus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eucalyptus.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:26:11 2026 GMT\n  hsts: false\ndomains:\n- domain: eucalyptus.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eucalyptus/refs/heads/main/security/eucalyptus-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthtech
- Telehealth
- Digital Health
- Telemedicine
- Weight Management
- Women's Health
- Men's Health
- Dermatology
- Reproductive Health
- Australia
---
