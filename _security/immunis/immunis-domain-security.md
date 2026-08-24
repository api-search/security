---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: immunisbiomedical.com
  spf: true
hosts:
- cert_expires: Sep 23 10:09:52 2026 GMT
  host: immunisbiomedical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Immunis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Immunis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Immunis
provider_slug: immunis
slug: immunis-domain-security
source_filename: immunis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: immunisbiomedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 10:09:52 2026 GMT\n  hsts: false\ndomains:\n- domain: immunisbiomedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/immunis/refs/heads/main/security/immunis-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Life Sciences
- Therapeutics
- Clinical Trials
- Regenerative Medicine
- Healthcare
- Longevity
- Sarcopenia
---
