---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: contractorforeman.com
  spf: true
hosts:
- cert_expires: Sep 23 04:32:49 2026 GMT
  host: contractorforeman.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 16:43:35 2026 GMT
  host: kb.contractorforeman.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Contractorforeman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contractor Foreman, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Contractor Foreman
provider_slug: contractorforeman
slug: contractorforeman-domain-security
source_filename: contractorforeman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contractorforeman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 04:32:49 2026 GMT\n  hsts: false\n- host: kb.contractorforeman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 16:43:35 2026 GMT\n  hsts: false\ndomains:\n- domain: contractorforeman.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contractorforeman/refs/heads/main/security/contractorforeman-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Construction
- Construction Management
- Contractor Software
- Estimating
- Invoicing
- Scheduling
---
