---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ushphealth.com
  spf: true
hosts:
- cert_expires: Sep 28 13:39:20 2026 GMT
  host: www.ushphealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Health Partners Llc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Health Partners, LLC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: US Health Partners, LLC
provider_slug: us-health-partners-llc
slug: us-health-partners-llc-domain-security
source_filename: us-health-partners-llc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ushphealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:39:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ushphealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-health-partners-llc/refs/heads/main/security/us-health-partners-llc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Cardiology
- Cardiovascular Care
- Physician Network
- Medical Practices
---
