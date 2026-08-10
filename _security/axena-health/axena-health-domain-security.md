---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: axenahealth.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: levacares.com
  spf: true
  spf_record: v=spf1 include:us._netblocks.mimecast.com include:_spf.salesforce.com include:spf.protection.outlook.com -all
hosts:
- cert_expires: Sep 16 06:49:52 2026 GMT
  host: axenahealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 22:55:19 2026 GMT
  host: levacares.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axena Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axena Health, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Axena Health
provider_slug: axena-health
slug: axena-health-domain-security
source_filename: axena-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axenahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:49:52 2026 GMT\n  hsts: false\n- host: levacares.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 22:55:19 2026 GMT\n  hsts: false\ndomains:\n- domain: axenahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: levacares.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:us._netblocks.mimecast.com include:_spf.salesforce.com\n    include:spf.protection.outlook.com -all\n  dmarc: true\n  dmarc_policy: reject\nx-note: >-\n  levacares.com was probed by hand because provider_hosts() only walks Website /\n  Portal pointers and API hosts; it is carried in apis.yml as ProductWebsite. It\n  is the host that serves the MCP endpoints and the OAuth discovery documents,\n  so its posture matters more\
  \ than the corporate site's. Neither host sets HSTS\n  and neither registrable domain is DNSSEC-signed or publishes a CAA record;\n  both publish SPF and a DMARC policy of p=reject.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axena-health/refs/heads/main/security/axena-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Digital Health
- Medical Devices
- Women's Health
- Digital Therapeutics
- Pelvic Health
- Medical Software
- Telehealth
---
