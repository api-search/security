---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crummy.com
  spf: true
hosts:
- cert_expires: Sep 28 20:16:37 2026 GMT
  host: www.crummy.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Beautiful Soup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beautiful Soup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Beautiful Soup
provider_slug: beautiful-soup
slug: beautiful-soup-domain-security
source_filename: beautiful-soup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crummy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 20:16:37 2026 GMT\n  hsts: false\ndomains:\n- domain: crummy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beautiful-soup/refs/heads/main/security/beautiful-soup-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Data Extraction
- HTML Parsing
- Python
- Scraping
- Web Scraping
- XML Parsing
---
