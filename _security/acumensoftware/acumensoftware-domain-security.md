---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acumensoft.net
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forcelink.net
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mysmart.city
  spf: true
hosts:
- cert_expires: Nov 10 10:59:56 2026 GMT
  host: www.acumensoft.net
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 05:27:53 2026 GMT
  host: www.forcelink.net
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 01:29:24 2026 GMT
  host: za2.forcelink.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 22:59:47 2026 GMT
  host: www.mysmart.city
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: app.mysmart.city
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 5
kind: domain-security
layout: security
method: probed
name: Acumensoftware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acumen Software, probed live across 5 host(s) and 3 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acumen Software
provider_slug: acumensoftware
slug: acumensoftware-domain-security
source_filename: acumensoftware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of every host in apis.yml (probe-domain-security.py), extended by hand with the\n  same probes for www.mysmart.city and app.mysmart.city, which the script did not reach\nnote: >-\n  No host publishes a CAA record and no domain is DNSSEC-signed. SPF and DMARC are present on all three\n  domains; only acumensoft.net enforces (p=quarantine), forcelink.net and mysmart.city are p=none. HSTS is\n  set on the three Wix-hosted marketing hosts and absent on both application hosts (za2.forcelink.net,\n  app.mysmart.city) — the hosts that actually carry the authenticated API traffic.\nhosts:\n- host: www.acumensoft.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 10:59:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: www.forcelink.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 05:27:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: za2.forcelink.net\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 01:29:24 2026 GMT\n  hsts: false\n- host: www.mysmart.city\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 22:59:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: app.mysmart.city\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: acumensoft.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: forcelink.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: mysmart.city\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acumensoftware/refs/heads/main/security/acumensoftware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Field Service Management
- Workforce Management
- Asset Management
- Enterprise Resource Planning
- Smart Cities
- Local Government
- Utilities
- Mobile
- South Africa
- MCP
---
