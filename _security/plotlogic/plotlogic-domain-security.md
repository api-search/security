---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: plotlogic.com
  spf: true
hosts:
- cert_expires: Aug 28 21:07:48 2026 GMT
  host: plotlogic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plotlogic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plotlogic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Plotlogic
provider_slug: plotlogic
slug: plotlogic-domain-security
source_filename: plotlogic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plotlogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 21:07:48 2026 GMT\n  hsts: false\ndomains:\n- domain: plotlogic.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plotlogic/refs/heads/main/security/plotlogic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mining
- Artificial Intelligence
- Sensors
- Material Characterisation
- Geoscience
- Industrial
- Machine Learning
---
