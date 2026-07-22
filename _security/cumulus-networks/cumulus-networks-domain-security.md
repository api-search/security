---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cumulusnetworks.com
  spf: true
hosts:
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: cumulusnetworks.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cumulus Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cumulus Networks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cumulus Networks
provider_slug: cumulus-networks
slug: cumulus-networks-domain-security
source_filename: cumulus-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cumulusnetworks.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cumulusnetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cumulus-networks/refs/heads/main/security/cumulus-networks-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Networking
- Network Operating System
- Linux
- Data Center
- Switching
- Open Networking
- Telemetry
---
