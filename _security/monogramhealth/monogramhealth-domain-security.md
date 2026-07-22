---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: monogramhealth.com
  spf: true
hosts:
- cert_expires: Oct 10 17:15:51 2026 GMT
  host: monogramhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Monogramhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monogramhealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Monogramhealth
provider_slug: monogramhealth
slug: monogramhealth-domain-security
source_filename: monogramhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monogramhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 17:15:51 2026 GMT\n  hsts: false\ndomains:\n- domain: monogramhealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monogramhealth/refs/heads/main/security/monogramhealth-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Value-Based Care
- Kidney Care
- Chronic Disease
- In-Home Care
- Nephrology
---
