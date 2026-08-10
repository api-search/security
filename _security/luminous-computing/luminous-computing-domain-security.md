---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: true
  domain: lmns.com
  mx: google-workspace
  note: No CAA record and no _dmarc TXT record are published. DNS is hosted on Google Cloud DNS and carries live Google Workspace MX plus Atlassian, Smartsheet and DocuSign domain-verification TXT records, so the domain is actively operated even though the public website has expired.
  spf: true
  spf_record: v=spf1 include:_spf.google.com ~all
hosts:
- cert_expires: Oct  3 08:12:14 2026 GMT
  host: lmns.com
  hsts: true
  hsts_max_age: 15552000
  http_status: 404
  https: true
  note: Squarespace origin. The apex returns HTTP 404 with the Squarespace "Website Expired" system page - the marketing-site subscription has lapsed. TLS and HSTS are still served by the Squarespace edge.
  tls_version: TLSv1.3
- host: luminous-co.squarespace.com
  hsts: false
  hsts_max_age: 0
  http_status: 200
  https: true
  note: Squarespace platform address for the same site; still serves the Luminous marketing page. Sends Strict-Transport-Security with max-age=0, i.e. HSTS explicitly disabled. This host is Squarespace-controlled infrastructure rather than a Luminous-registered domain, so its posture is not attributable to the company.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Luminous Computing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luminous Computing, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Luminous Computing
provider_slug: luminous-computing
slug: luminous-computing-domain-security
source_filename: luminous-computing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (probe-domain-security.py plus curl/dig verification)\nhosts:\n- host: lmns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:12:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  http_status: 404\n  note: >-\n    Squarespace origin. The apex returns HTTP 404 with the Squarespace \"Website Expired\"\n    system page - the marketing-site subscription has lapsed. TLS and HSTS are still served\n    by the Squarespace edge.\n- host: luminous-co.squarespace.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n  hsts_max_age: 0\n  http_status: 200\n  note: >-\n    Squarespace platform address for the same site; still serves the Luminous marketing page.\n    Sends Strict-Transport-Security with max-age=0, i.e. HSTS explicitly disabled. This host is\n    Squarespace-controlled infrastructure rather than a Luminous-registered domain, so its\n    posture is not attributable\
  \ to the company.\ndomains:\n- domain: lmns.com\n  dnssec: true\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com ~all\n  dmarc: false\n  dmarc_policy: null\n  mx: google-workspace\n  note: >-\n    No CAA record and no _dmarc TXT record are published. DNS is hosted on Google Cloud DNS and\n    carries live Google Workspace MX plus Atlassian, Smartsheet and DocuSign domain-verification\n    TXT records, so the domain is actively operated even though the public website has expired.\nx-evidence:\n  fetched: '2026-08-04'\n  dns_method: dig +short A/NS/MX/TXT/CAA and dig +short TXT _dmarc.lmns.com\n  tls_method: TLS handshake on port 443 plus curl -sI for response headers\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luminous-computing/refs/heads/main/security/luminous-computing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Semiconductors
- Silicon Photonics
- Photonic Computing
- Optical Interconnect
- AI Accelerators
- Artificial Intelligence
- High Performance Computing
- Hardware
- Deep Tech
- United States
---
