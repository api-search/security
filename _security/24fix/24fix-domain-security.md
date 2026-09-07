---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 24x.co.th
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 24fix.co
  note: DMARC record is GoDaddy parking infrastructure (rua=dmarc_rua@onsecureserver.net), not a policy the company publishes for its operating domain.
  spf: false
hosts:
- cert_expires: Oct 20 00:30:12 2026 GMT
  host: 24x.co.th
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 00:30:12 2026 GMT
  host: www.24x.co.th
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 00:30:12 2026 GMT
  host: fix.24x.co.th
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 00:30:12 2026 GMT
  host: business.24x.co.th
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 00:30:12 2026 GMT
  host: housesolution.24x.co.th
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 00:30:12 2026 GMT
  host: projects.24x.co.th
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 00:30:12 2026 GMT
  host: careers.24x.co.th
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 12 11:47:00 2027 GMT
  host: 24fix.co
  hsts: false
  https: true
  note: parked domain (GoDaddy), not an operated site
  tls_version: TLSv1.3
hosts_probed: 8
kind: domain-security
layout: security
method: probed
name: 24Fix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 24 FIX, probed live across 8 host(s) and 2 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: 24 FIX
provider_slug: 24fix
slug: 24fix-domain-security
source_filename: 24fix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every 24X / 24 FIX host reachable from apis.yml\nnote: >-\n  All 24x.co.th hosts sit behind Cloudflare and share one wildcard certificate. The legacy\n  24fix.co brand domain is no longer operated as a site — it resolves to GoDaddy parking\n  (ns07/ns08.domaincontrol.com, /lander redirect stub) and is recorded here only because it\n  is the brand's historic domain and is still linked from 24x.co.th.\nhosts:\n- host: 24x.co.th\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 00:30:12 2026 GMT\n  hsts: false\n- host: www.24x.co.th\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 00:30:12 2026 GMT\n  hsts: false\n- host: fix.24x.co.th\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 00:30:12 2026 GMT\n  hsts: false\n- host: business.24x.co.th\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 00:30:12 2026 GMT\n  hsts: false\n- host: housesolution.24x.co.th\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 00:30:12 2026 GMT\n  hsts: false\n- host: projects.24x.co.th\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 00:30:12 2026 GMT\n  hsts: false\n- host: careers.24x.co.th\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 00:30:12 2026 GMT\n  hsts: false\n- host: 24fix.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 11:47:00 2027 GMT\n  hsts: false\n  note: parked domain (GoDaddy), not an operated site\ndomains:\n- domain: 24x.co.th\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: 24fix.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n  note: >-\n    DMARC record is GoDaddy parking infrastructure (rua=dmarc_rua@onsecureserver.net), not a\n    policy the company publishes for its operating domain.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/24fix/refs/heads/main/security/24fix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Home Services
- Property Maintenance
- Facility Management
- Field Service
- Marketplace
- Construction
- Renovation
- Consumer Services
- Thailand
- Southeast Asia
---
