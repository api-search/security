---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dcma.mil
  spf: true
hosts:
- cert_expires: Aug 17 15:25:38 2026 GMT
  host: www.dcma.mil
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Defense Contract Management Agency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defense Contract Management Agency, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Defense Contract Management Agency
provider_slug: defense-contract-management-agency
slug: defense-contract-management-agency-domain-security
source_filename: defense-contract-management-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dcma.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 15:25:38 2026 GMT\n  hsts: null\ndomains:\n- domain: dcma.mil\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defense-contract-management-agency/refs/heads/main/security/defense-contract-management-agency-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Defense
- Department of Defense
- Contract Management
- Acquisition
- Earned Value Management
---
