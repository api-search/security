---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issuewild "amazon.com"
  dmarc: false
  dnssec: false
  domain: navitia.io
  spf: true
hosts:
- cert_expires: Sep 29 10:07:49 2026 GMT
  host: doc.navitia.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Navitia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Navitia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Navitia
provider_slug: navitia
slug: navitia-domain-security
source_filename: navitia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doc.navitia.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:07:49 2026 GMT\n  hsts: false\ndomains:\n- domain: navitia.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navitia/refs/heads/main/security/navitia-domain-security.yml
summary_line: TLSv1.3
tags:
- Transportation
- Public APIs
---
