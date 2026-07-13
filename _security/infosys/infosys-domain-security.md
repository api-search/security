---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: infosys.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openbankproject.com
  spf: true
hosts:
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: www.infosys.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: infosys-finacle.openbankproject.com
  https: false
kind: domain-security
layout: security
method: probed
name: Infosys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infosys, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Infosys
provider_slug: infosys
slug: infosys-domain-security
source_filename: infosys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.infosys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\n- host: infosys-finacle.openbankproject.com\n  https: false\ndomains:\n- domain: infosys.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: openbankproject.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infosys/refs/heads/main/security/infosys-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- IT Services
- Consulting
- Banking
- Open Banking
- Finacle
- Digital Transformation
- Cloud
---
