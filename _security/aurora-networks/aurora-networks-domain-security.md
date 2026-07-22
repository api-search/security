---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: auroranetworks.com
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com -all
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vistancenetworks.com
  spf: true
hosts:
- cert_expires: Oct  3 08:27:56 2026 GMT
  host: www.vistancenetworks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: auroranetworks.com
  hsts: false
  https: true
  note: brand domain; redirects to https://www.vistancenetworks.com/
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aurora Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aurora Networks, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aurora Networks
provider_slug: aurora-networks
slug: aurora-networks-domain-security
source_filename: aurora-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vistancenetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:27:56 2026 GMT\n  hsts: false\n- host: auroranetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: false\n  note: brand domain; redirects to https://www.vistancenetworks.com/\ndomains:\n- domain: auroranetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com -all\n  dmarc: false\n- domain: vistancenetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aurora-networks/refs/heads/main/security/aurora-networks-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Networking
- Broadband
- Telecommunications
- Cable
- Fiber Optics
- Access Networks
- Network Infrastructure
- Hardware
- Service Assurance
---
