---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iralogix.com
  spf: true
hosts:
- cert_expires: Sep 11 23:02:25 2026 GMT
  host: iralogix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: partner.iralogix.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  8 13:20:14 2026 GMT
  host: auth.partner.iralogix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iralogix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IRALOGIX, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IRALOGIX
provider_slug: iralogix
slug: iralogix-domain-security
source_filename: iralogix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iralogix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:02:25 2026 GMT\n  hsts: false\n- host: partner.iralogix.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: false\n- host: auth.partner.iralogix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 13:20:14 2026 GMT\n  hsts: false\ndomains:\n- domain: iralogix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iralogix/refs/heads/main/security/iralogix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial-Services
- Retirement
- IRA
- Recordkeeping
- Wealth Management
- Fintech
- Compliance
- White Label
- Retirement Technology
---
