---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: acrivon.com
  spf: true
hosts:
- cert_expires: Jan 13 05:13:43 2027 GMT
  host: acrivon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Acrivon Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acrivon Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Acrivon Therapeutics
provider_slug: acrivon-therapeutics
slug: acrivon-therapeutics-domain-security
source_filename: acrivon-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acrivon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 05:13:43 2027 GMT\n  hsts: false\ndomains:\n- domain: acrivon.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/acrivon-therapeutics/security/acrivon-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Oncology
- Biotechnology
- Precision Medicine
- Therapeutics
---
