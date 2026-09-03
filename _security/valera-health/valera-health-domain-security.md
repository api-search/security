---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: valerahealth.com
  spf: true
hosts:
- cert_expires: Oct 17 19:25:48 2026 GMT
  host: www.valerahealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Valera Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valera Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Valera Health
provider_slug: valera-health
slug: valera-health-domain-security
source_filename: valera-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.valerahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 19:25:48 2026 GMT\n  hsts: false\ndomains:\n- domain: valerahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valera-health/refs/heads/main/security/valera-health-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Health
- Healthcare
- Behavioral Health
- Mental Health
- Telehealth
- Telemedicine
- Psychiatry
- Digital Health
---
