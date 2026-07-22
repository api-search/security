---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:wafadmin@fireeye.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: false
  dnssec: true
  domain: mandiant.com
  spf: true
hosts:
- cert_expires: Oct 14 04:01:48 2026 GMT
  host: docs.mandiant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 13:45:32 2026 GMT
  host: api.intelligence.mandiant.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mandiant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mandiant, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Mandiant
provider_slug: mandiant
slug: mandiant-domain-security
source_filename: mandiant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.mandiant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 04:01:48 2026 GMT\n  hsts: false\n- host: api.intelligence.mandiant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 13:45:32 2026 GMT\n  hsts: null\ndomains:\n- domain: mandiant.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:wafadmin@fireeye.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mandiant/refs/heads/main/security/mandiant-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Security
- Threat Intelligence
- Cybersecurity
- Incident Response
- Attack Surface Management
- Vulnerability Intelligence
- Malware
- Google Cloud
---
