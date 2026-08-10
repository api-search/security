---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eton-solutions.com
  spf: true
hosts:
- cert_expires: Oct 27 12:01:07 2026 GMT
  host: eton-solutions.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eton Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eton Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eton Solutions
provider_slug: eton-solutions
slug: eton-solutions-domain-security
source_filename: eton-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eton-solutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 12:01:07 2026 GMT\n  hsts: null\ndomains:\n- domain: eton-solutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eton-solutions/refs/heads/main/security/eton-solutions-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Family Office
- Wealth Management
- Wealth Technology
- ERP
- Financial Software
- Accounting
- Artificial Intelligence
- Private Wealth
- Fintech
---
