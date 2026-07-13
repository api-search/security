---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dsca.mil
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dscu.edu
  spf: true
hosts:
- cert_expires: Jul 29 18:07:45 2026 GMT
  host: www.dsca.mil
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: www.dscu.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Defense Security Cooperation Agency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defense Security Cooperation Agency, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Defense Security Cooperation Agency
provider_slug: defense-security-cooperation-agency
slug: defense-security-cooperation-agency-domain-security
source_filename: defense-security-cooperation-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dsca.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 29 18:07:45 2026 GMT\n  hsts: null\n- host: www.dscu.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dsca.mil\n  dnssec: true\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: dscu.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defense-security-cooperation-agency/refs/heads/main/security/defense-security-cooperation-agency-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Defense
- Department of Defense
- DSCA
- Federal Government
- Foreign Military Sales
- International
- Security Cooperation
---
