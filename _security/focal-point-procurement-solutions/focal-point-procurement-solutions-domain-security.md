---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getfocalpoint.com
  spf: true
hosts:
- cert_expires: Sep 21 22:59:52 2026 GMT
  host: getfocalpoint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Focal Point Procurement Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Focal Point Procurement Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Focal Point Procurement Solutions
provider_slug: focal-point-procurement-solutions
slug: focal-point-procurement-solutions-domain-security
source_filename: focal-point-procurement-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getfocalpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 22:59:52 2026 GMT\n  hsts: false\ndomains:\n- domain: getfocalpoint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/focal-point-procurement-solutions/refs/heads/main/security/focal-point-procurement-solutions-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Procurement
- Source-to-Pay
- Supplier Management
- Contract Lifecycle Management
- Third-Party Risk
- Spend Management
- Enterprise SaaS
---
