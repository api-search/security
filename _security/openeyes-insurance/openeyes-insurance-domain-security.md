---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openeyes.com
  spf: true
hosts:
- cert_expires: Sep 17 09:42:47 2026 GMT
  host: openeyes.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openeyes Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenEyes Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenEyes Insurance
provider_slug: openeyes-insurance
slug: openeyes-insurance-domain-security
source_filename: openeyes-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openeyes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 09:42:47 2026 GMT\n  hsts: false\ndomains:\n- domain: openeyes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openeyes-insurance/refs/heads/main/security/openeyes-insurance-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Insurance
- Insurtech
- Commercial Auto Insurance
- Fleet Management
- Telematics
- Risk Management
---
