---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arrive.com
  spf: true
hosts:
- cert_expires: Mar 24 23:59:59 2027 GMT
  host: arrive.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arrive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arrive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arrive
provider_slug: arrive
slug: arrive-domain-security
source_filename: arrive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arrive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 24 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: arrive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arrive/refs/heads/main/security/arrive-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Mobility
- SmartCities
- Parking
- Transportation
- SaaS
- Company
---
