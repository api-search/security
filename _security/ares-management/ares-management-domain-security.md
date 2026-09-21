---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aresmgmt.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ares.com
  note: No SPF TXT record observed at the apex on 2026-09-18 (DMARC is published via Proofpoint).
  spf: false
hosts:
- cert_expires: Dec  4 06:48:52 2026 GMT
  host: www.aresmgmt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 12:12:49 2026 GMT
  host: www.ares.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  note: Current corporate host; aresmgmt.com redirects here.
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Ares Management Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ares Management, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ares Management
provider_slug: ares-management
slug: ares-management-domain-security
source_filename: ares-management-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts, extended by hand on 2026-09-18 to www.ares.com\n  / ares.com, the current corporate domain that aresmgmt.com now 301s to\nhosts:\n- host: www.aresmgmt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 06:48:52 2026 GMT\n  hsts: null\n- host: www.ares.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 12:12:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n  note: Current corporate host; aresmgmt.com redirects here.\ndomains:\n- domain: aresmgmt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ares.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n  note: No SPF TXT record observed at the apex on 2026-09-18 (DMARC is published via Proofpoint).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ares-management/refs/heads/main/security/ares-management-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Alternative Investment
- Credit
- Private Equity
- Real-Estate
- Infrastructure
- Asset Management
- Secondaries
- Financial-Services
---
