---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nextbank.holiday
  spf: false
hosts:
- cert_expires: Dec 31 10:38:37 2026 GMT
  host: nextbank.holiday
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: nextbank.holiday Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nextbank.holiday, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: nextbank.holiday
provider_slug: nextbank-holiday
slug: nextbank-holiday-domain-security
source_filename: nextbank-holiday-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nextbank.holiday\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 10:38:37 2026 GMT\n  hsts: false\ndomains:\n- domain: nextbank.holiday\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nextbank-holiday/security/nextbank-holiday-domain-security.yml
summary_line: TLSv1.3
tags:
- BankHoliday
- United Kingdom
- Europe
- Calendar
---
